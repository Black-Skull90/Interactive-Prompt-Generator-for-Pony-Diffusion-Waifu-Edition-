<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Prompt Generator for Pony Diffusion (Waifu Edition) - README</title>
    <style>
        body {
            font-family: sans-serif;
            line-height: 1.6;
            margin: 20px;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }
        h1, h2 {
            border-bottom: 1px solid #eaecef;
            padding-bottom: 0.3em;
        }
        h1 { font-size: 2em; }
        h2 { font-size: 1.5em; }
        ul { padding-left: 20px; }
        li { margin-bottom: 0.5em; }
        code {
            font-family: monospace;
            background-color: #f6f8fa;
            padding: 0.2em 0.4em;
            margin: 0;
            font-size: 85%;
            border-radius: 3px;
        }
        p { margin-bottom: 1em; }
    </style>
</head>
<body>

    <h1>Interactive Prompt Generator for Pony Diffusion (Waifu Edition)</h1>

    <p>This project is an interactive webpage designed to facilitate the creation of detailed prompts for image generation models based on Pony Diffusion, with a focus on creating "waifu" characters. The tool allows users to visually configure a wide range of characteristics, actions, and scenarios, automatically generating the corresponding positive and negative prompts, ready to be used on platforms like SeaArt.ai or others that support the Pony Diffusion model.</p>

    <h2>How It Was Made</h2>
    <ul>
        <li><strong>HTML:</strong> Semantic structure of the page.</li>
        <li><strong>CSS (Tailwind CSS):</strong> Modern, responsive, and customizable styling, including light and dark themes.</li>
        <li><strong>JavaScript (Pure/Vanilla):</strong> Responsible for all interactivity, including:
            <ul>
                <li>Dynamic updating of prompts based on user selections.</li>
                <li>State management for options (SFW/NSFW, language, theme).</li>
                <li>DOM manipulation to show/hide contextual sections (such as advanced NSFW controls).</li>
                <li>Copy-to-clipboard functionality.</li>
                <li>Internationalization (i18n) for switching between Portuguese and English in the interface.</li>
                <li>Warning modal for sensitive content.</li>
            </ul>
        </li>
    </ul>

    <h2>Fundamentals</h2>
    <p>The core idea is to simplify the often complex process of "prompt engineering" for generative AI models. Instead of manually typing long strings of tags, the user interacts with an intuitive graphical interface (dropdown menus, checkboxes, switches), and the tool translates these choices into prompts optimized for Pony Diffusion.</p>
    <p>The system uses common and recommended tags for the model, including:</p>
    <ul>
        <li><code>score_tags</code> for quality.</li>
        <li><code>source_tags</code> for the main artistic style.</li>
        <li><code>rating_tags</code> for content classification (SFW/NSFW).</li>
        <li>A wide range of tags for physical appearance, clothing, accessories, actions, poses, expressions, scenarios, and NSFW details.</li>
    </ul>

    <h2>How It Works</h2>
    <ol>
        <li><strong>User Interface:</strong> The user navigates through different sections and selects the desired options for their character.</li>
        <li><strong>Language and Theme Selection:</strong> Controls at the top of the page allow customization of the visual experience and interface language.</li>
        <li><strong>NSFW Mode:</strong> When "NSFW" is selected, a warning modal is displayed (with an option to not show it again). If the user proceeds, additional sections with detailed NSFW controls become visible.</li>
        <li><strong>Dynamic Prompt Generation:</strong> Each interaction with a control (click, selection) triggers a JavaScript function that:
            <ul>
                <li>Collects the values from all relevant fields.</li>
                <li>Adds the corresponding tags to a positive prompt array.</li>
                <li>Adds exclusion tags (negative) based on selections (e.g., if SFW, adds NSFW tags to the negative prompt).</li>
                <li>Filters out duplicate or empty tags.</li>
            </ul>
        </li>
        <li><strong>Display and Copy:</strong> The positive and negative prompts are displayed in real-time in separate text boxes. "Copy" buttons allow the user to easily transfer them to the clipboard.</li>
        <li><strong>Reset:</strong> A "Reset to Defaults" button restores all selections to a predefined initial state.</li>
    </ol>

    <h2>Applications</h2>
    <ul>
        <li><strong>Image Generation:</strong> Primarily for creating prompts for the Pony Diffusion model on AI art generation platforms (e.g., SeaArt.ai, Stable Diffusion WebUI with the Pony model).</li>
        <li><strong>Tag Learning:</strong> Users can learn which tags are effective for different characteristics and styles.</li>
        <li><strong>Rapid Experimentation:</strong> Allows for quick testing of different prompt combinations without extensive manual typing.</li>
        <li><strong>Basis for More Complex Tools:</strong> The code can serve as a foundation for developing more advanced prompt generators or integrating with other systems.</li>
    </ul>
    <p>This generator aims to make AI art creation more accessible and fun, especially for those focusing on anime style and detailed character customization.</p>

    <h2>How to Use</h2>
    <ol>
        <li>Clone or download this repository.</li>
        <li>Open the <code>Waifu_generator_pony_diffusion.html</code> file in your web browser.</li>
        <li>Use the interactive controls to select features for your character.</li>
        <li>Copy the generated positive and negative prompts.</li>
        <li>Paste them into your preferred AI image generation platform that supports Pony Diffusion.</li>
    </ol>

    <hr>

</body>
</html>
