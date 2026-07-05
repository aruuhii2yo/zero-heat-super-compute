# Installation Guide

## Option 1 — Cloud via Smithery (recommended, no install)

1. Open https://smithery.ai/servers/aruuhii2yo/maxion-mcp-gateway
2. Click **Connect** and follow the prompts for your client (Claude Desktop, Cursor, etc.)
3. If you've purchased a license, paste your Gumroad license key when prompted. Leave it blank to use the free 30-minute trial.

All 19 tools are available immediately.

## Option 2 — Cloud via direct endpoint

Add this to any MCP client that supports Streamable HTTP:

```
https://5pu357jdkqc3qynzkjvu3okgqy0ncsiy.lambda-url.us-east-1.on.aws/mcp
```

To use a purchased license, send it in the `x-fleet-key` header or append `?licenseKey=YOUR_KEY` to the URL.

## Option 3 — Local engines (Windows, license required)

Runs the Maxion / Diamonize / Quezar engines natively on your machine. Requires **Node.js 18+** and a valid Gumroad license key. Your package contains only the engine(s) your license covers.

**1. Request your personalized package:**

```bash
curl -X POST https://5pu357jdkqc3qynzkjvu3okgqy0ncsiy.lambda-url.us-east-1.on.aws/download-package \
  -H "Content-Type: application/json" \
  -d '{"license_key":"YOUR_LICENSE_KEY"}'
```

The response contains a `download_url` valid for 1 hour.

**2. Download and unpack:**

```bash
curl -o maxion-mcp-gateway.zip "<download_url from step 1>"
unzip maxion-mcp-gateway.zip
cd maxion-mcp-gateway
npm install
```

**3. Add to your Claude Desktop config** (`claude_desktop_config.json`):

```json
{
  "mcpServers": {
    "maxion": {
      "command": "node",
      "args": ["/absolute/path/to/maxion-mcp-gateway/mcp_wrapper.js"]
    }
  }
}
```

Restart Claude Desktop. Your licensed engine tools now run locally.

## Getting a license

Call the `billing.purchase` tool from your connected AI client for a direct Gumroad checkout link, or visit [advancedapparchitect.com](https://advancedapparchitect.com). Your license key arrives in the Gumroad receipt email immediately after purchase.

## Support

- Enterprise & fleet licensing: **aruuh@advancedapparchitect.com**
- Website: https://advancedapparchitect.com
