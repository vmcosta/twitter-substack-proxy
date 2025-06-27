# Twitter Substack Proxy Setup

This app creates proxy pages for Substack articles to work around Twitter's artificial limitations on Substack links.

## Setup Complete ✅

The app has been successfully set up with:
- ✅ Repository cloned from https://github.com/OmarShehata/twitter-substack-proxy
- ✅ Dependencies installed using pnpm
- ✅ Environment variables configured (PORT=3000)
- ✅ Server tested and working

## Available Commands

```bash
# Add pnpm to PATH (run this in each new terminal session)
export PATH="$HOME/.npm-global/bin:$PATH"

# Set environment variables
source env.sh
# or manually: export PORT=3000

# Start the server (production)
pnpm start

# Start with auto-reload (development)
pnpm watch
```

## Usage

1. Start the server:
   ```bash
   export PATH="$HOME/.npm-global/bin:$PATH"
   export PORT=3000
   pnpm start
   ```

2. Visit http://localhost:3000 in your browser

3. Enter a Substack URL to generate a proxy link

4. Share the proxy link on Twitter instead of the original Substack link

## How it Works

- Creates HTML pages with proper meta tags that Twitter will display as preview cards
- Redirects to the original Substack article after the meta tags load
- Bypasses Twitter's artificial reach limitations on Substack links

## Railway Deployment ✅

The app has been deployed to Railway at:
**https://illuminate.up.railway.app/**

### Railway Commands
```bash
# Check deployment status
railway status

# View logs
railway logs

# Generate new domain (if needed)
railway domain
```

## Project Structure

- `src/server.js` - Main server code
- `views/` - Handlebars templates
- `public/` - Static assets
- `package.json` - Dependencies and scripts 