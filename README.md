### Crafting a Custom GPT for Shad UI: A Step-by-Step Guide

If you\'re interested in creating a specialized GPT for Shad UI, follow this comprehensive how-to guide:

1. **Set Up the Foundation**: Begin by setting up the necessary infrastructure using the [GPT Crawler](https://github.com/BuilderIO/gpt-crawler). This tool is essential for gathering the data required to train your custom gpt.

2. **Curate Data**: After running the crawler, review the generated `.json` file. Initially, you might find that the HTML output lacks depth. For example:
    ```json
    {
      "title": "Alert - shadcn/ui",
      "url": "https://ui.shadcn.com/docs/components/alert",
      "html": "npx shadcn-ui@latest add alert"
    }
    ```

3. **Enhance Content Quality**: To improve the GPT's learning material, manually visit relevant URLs, such as the [Shad UI Alert Component](https://ui.shadcn.com/docs/components/alert), and replace simplistic HTML with detailed code blocks like this:
    ```json
    {
      "title": "Alert - shadcn/ui",
      "url": "https://ui.shadcn.com/docs/components/alert",
      "html": "<Alert>...</Alert>"
    }
    ```

4. **Refine Instructions**: Craft precise instructions for the GPT . Emphasize a focus on ShadUI components, frontend development, and specific use cases. These instructions help the gpt understand its specialized role.


