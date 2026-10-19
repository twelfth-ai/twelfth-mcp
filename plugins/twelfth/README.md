# Twelfth

Connects Claude to a [Twelfth](https://twelfth.ai) workspace and adds eight
skills for retail and category work.

## What it connects to

One remote MCP server, `https://api.twelfth.ai/mcp` (Streamable HTTP), run by
Twelfth AI Pty Ltd. You sign in with your Twelfth account through OAuth 2.1,
choose one workspace and approve the tools the connection may use. The plugin
holds no credentials and runs nothing on your machine.

The server reads the products, suppliers, sales, inventory, pricing, projects
and actions you can already see in Twelfth, within your role and remits. It
changes nothing unless you tick **Allow changes** when connecting. Then it can
create, complete or snooze your own actions and run your own routines, as you.
No tool raises an order or changes a price. Owners and admins can see and end
any connection from **Settings → AI & agents**.

The plugin sends nothing anywhere else. Tool calls go only to the server above.

## Skills

Retail analysis. These work on a spreadsheet or pasted data, with no Twelfth
account:

- `sales-decline-diagnosis`: why sales of a category, supplier or product fell
- `category-review`: a category's role, scorecard, availability, return on stock, range and promotions
- `range-review`: which lines to keep, cut or add
- `supplier-offer-review`: what to buy from a supplier's stock list or offer, and how much
- `competitor-price-check`: price position on matched products, and whether to match

Twelfth. These use the connection:

- `twelfth-workspace`: getting started, what the tools can see, how changes work
- `twelfth-weekly-trading-brief`: Monday's brief, with actions due, suppliers waiting, cover pressure and prices
- `twelfth-competitor-pricing`: tracked sets, competitor comparisons and price history

## Requirements

A Twelfth workspace. [Book a demo](https://twelfth.ai/book-a-demo) if your team
doesn't have one. The retail analysis skills work without it.

## Support

hello@twelfth.ai · [Docs](https://twelfth.ai/developers/mcp) · [Privacy](https://twelfth.ai/legals/privacy) · [Trust centre](https://trust.twelfth.ai)

Licensed MIT.
