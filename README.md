Interactive Prompt Generator for Pony Diffusion (Waifu Edition)
This project is an interactive webpage designed to facilitate the creation of detailed prompts for image generation models based on Pony Diffusion, with a focus on creating "waifu" style characters. The tool allows users to visually configure a wide range of characteristics, actions, and scenarios, automatically generating the corresponding positive and negative prompts, ready to be used on platforms like SeaArt.ai or others that support the Pony Diffusion model.

Interface Overview
The interface is divided into sections to make it easy to configure your character and scene:

Top Controls:

Language Selector: Switch the interface between Portuguese, English, Japanese, and Spanish.

Theme Toggle: Choose between a light (default) or dark theme.

General Settings:

Rating: Define as SFW (safe for work) or NSFW (not safe for work).

Source (Main Style): Choose the base style of the image (Anime, Furry, Cartoon, Pony).

Number of Characters: Specify how many girls will be in the image.

Artistic Style:

Main Style: Select a predominant artistic technique (Oil Painting, Watercolor, etc.).

Appearance:

Details such as species, hair (color and style), eyes (color), and skin tone (with an option for tanned skin).

Body:

Define the age range (Young Adult, Adult, Mature, MILF), build, and bust size.

Clothing & Accessories:

Select the main outfit and various accessories.

Daily Actions:

Choose an everyday activity for the character.

Specific NSFW Settings:

Visible only if "NSFW" is selected. Includes an 18+ content warning and options for sensual poses, actions, objects, intimate details, etc.

Pose & Expression:

Define the character's posture and facial expression.

Scenario:

Select the environment and lighting type.

Additional Art Quality (Positive):

Tags to improve the overall image quality (Masterpiece, Best Quality, etc.).

AI Assistance (Gemini):

Enhance Positive Prompt with AI: The AI suggests additional tags for your prompt.

Generate Character Idea with AI: The AI generates a list of Danbooru-style tags based on your selections.

Generated Prompts:

Displays the positive and negative prompts, with buttons to copy.

Reset:

Button to return all options to their initial values.

Footer:

"Developed by BlackSkull90" indication.

How to Use
Clone or download this repository.

Open the Waifu_generator_pony_diffusion.html file in your web browser.

Use the interactive controls to select the characteristics of your character and scene.

Copy the positive and negative prompts generated in the text boxes.

Paste the prompts into your preferred AI image generation platform that supports Pony Diffusion (e.g., SeaArt.ai).

Technologies Used
HTML: Page structure.

CSS (Tailwind CSS): Styling and responsiveness.

JavaScript (Pure): Interactivity, prompt generation, theme and language management, and Gemini API calls.

Main Features
Intuitive graphical interface for selecting dozens of attributes.

Dynamic generation of positive and negative prompts optimized for Pony Diffusion.

Support for multiple languages (Portuguese, English, Japanese, Spanish).

Light and dark themes.

Dedicated section for NSFW settings with a content warning.

Integration with the Gemini API to:

Suggest additional tags to enrich the positive prompt.

Generate character ideas in Danbooru tag format.

Functionality to copy prompts to the clipboard.

Option to reset all settings.

Quick Tips
Experiment! The best way to learn is to test different combinations.

Start with fewer options and gradually add details.

The translations for Japanese and Spanish are automatic and may need review for greater naturalness.

Developed by BlackSkull90
