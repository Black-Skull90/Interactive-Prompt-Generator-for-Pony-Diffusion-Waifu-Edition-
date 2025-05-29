Interactive Prompt Generator for Pony Diffusion (Waifu Edition)
This project is an interactive webpage designed to facilitate the creation of detailed prompts for image generation models based on Pony Diffusion, with a focus on creating "waifu" characters. The tool allows users to visually configure a wide range of characteristics, actions, and scenarios, automatically generating the corresponding positive and negative prompts, ready to be used on platforms like SeaArt.ai or others that support the Pony Diffusion model.
How It Was Made
 * HTML: Semantic structure of the page.
 * CSS (Tailwind CSS): Modern, responsive, and customizable styling, including light and dark themes.
 * JavaScript (Pure/Vanilla): Responsible for all interactivity, including:
   * Dynamic updating of prompts based on user selections.
   * State management for options (SFW/NSFW, language, theme).
   * DOM manipulation to show/hide contextual sections (such as advanced NSFW controls).
   * Copy-to-clipboard functionality.
   * Internationalization (i18n) for switching between Portuguese and English in the interface.
   * Warning modal for sensitive content.
Fundamentals
The core idea is to simplify the often complex process of "prompt engineering" for generative AI models. Instead of manually typing long strings of tags, the user interacts with an intuitive graphical interface (dropdown menus, checkboxes, switches), and the tool translates these choices into prompts optimized for Pony Diffusion.
The system uses common and recommended tags for the model, including:
 * score_tags for quality.
 * source_tags for the main artistic style.
 * rating_tags for content classification (SFW/NSFW).
 * A wide range of tags for physical appearance, clothing, accessories, actions, poses, expressions, scenarios, and NSFW details.
How It Works
 * User Interface: The user navigates through different sections and selects the desired options for their character.
 * Language and Theme Selection: Controls at the top of the page allow customization of the visual experience and interface language.
 * NSFW Mode: When "NSFW" is selected, a warning modal is displayed (with an option to not show it again). If the user proceeds, additional sections with detailed NSFW controls become visible.
 * Dynamic Prompt Generation: Each interaction with a control (click, selection) triggers a JavaScript function that:
   * Collects the values from all relevant fields.
   * Adds the corresponding tags to a positive prompt array.
   * Adds exclusion tags (negative) based on selections (e.g., if SFW, adds NSFW tags to the negative prompt).
   * Filters out duplicate or empty tags.
 * Display and Copy: The positive and negative prompts are displayed in real-time in separate text boxes. "Copy" buttons allow the user to easily transfer them to the clipboard.
 * Reset: A "Reset to Defaults" button restores all selections to a predefined initial state.
Applications
 * Image Generation: Primarily for creating prompts for the Pony Diffusion model on AI art generation platforms (e.g., SeaArt.ai, Stable Diffusion WebUI with the Pony model).
 * Tag Learning: Users can learn which tags are effective for different characteristics and styles.
 * Rapid Experimentation: Allows for quick testing of different prompt combinations without extensive manual typing.
 * Basis for More Complex Tools: The code can serve as a foundation for developing more advanced prompt generators or integrating with other systems.
This generator aims to make AI art creation more accessible and fun, especially for those focusing on anime style and detailed character customization.
How to Use
 * Clone or download this repository.
 * Open the Waifu_generator_pony_diffusion.html file in your web browser.
 * Use the interactive controls to select features for your character.
 * Copy the generated positive and negative prompts.
 * Paste them into your preferred AI image generation platform that supports Pony Diffusion.
This README was generated based on the project description.
