# Notion-CocktailDB-Integration
The following is an API integration of Notion and TheCocktailDB implementing Three-Legged OAuth where you are able to get cocktail recipes from TheCocktailDB, either random or by user input, that then adds them into your own Notion notebook you select.

## Requirements
- [Node.js](https://nodejs.org/en/download/current)
- Notion
    - Create or use existing workspace
        - Choose a page
        - Create or use an existing table/database
    - Create an [integration](https://developers.notion.com/docs/create-a-notion-integration) (make it public)
    - In the integration settings:
        - Fill out required information
        - Set Website or homepage to `http://localhost:3000/`
        - Redirect URI to `http://localhost:3000/auth/notion/callback`
    - Configure credentials.json
        - Copy OAuth client ID, OAuth client secret
        - Select a page you want to use, and get [database id](https://developers.notion.com/reference/retrieve-a-database)

## For further information on the Notion API, refer to [Notion Documentation](https://developers.notion.com/reference/intro)
## For further information on the CocktailDB API, refer to [CocktailDB Documentation](https://www.thecocktaildb.com/api.php)

