# Ascend.so for Claude

Adds one command to Claude, `/ascend`, for people who use Ascend. It answers from your own Ascend account's Instagram Reels data.

## What you need

- An Ascend account with an Instagram account added and a plan that can connect.
- A paid Claude plan, with "Code execution and file creation" switched on in Claude's settings.

The plugin brings the Ascend connector with it. After you add the plugin, open it under Customize > Plugins, go to its Connectors tab and connect Ascend, then sign in to your Ascend account. If you already connected Ascend from the MCP page in the Ascend app, that works too.

## What it sends

The plugin itself is one text file that tells Claude how to use Ascend's tools. It runs no code and sends nothing on its own. When you use it, Claude calls the Ascend connector at `https://mcp.ascend.so/mcp` with what the request needs: Reel links, @handles, search words, or a question for Ascend's own assistant. Ascend's answers use your account's Ascend credits, as in the app, and Claude asks before the first paid call. Ascend's privacy policy: https://ascend.so/privacy.

## Add it

On claude.ai or in the Claude desktop app:

1. Open Customize, then Plugins.
2. Choose Add, then Add marketplace, and enter `ascend-so/plugins`.
3. Add Ascend.so from the list, then connect Ascend on the plugin's Connectors tab if it isn't connected yet.

Start a new chat afterwards. To get later improvements without doing anything, turn on "Sync automatically" for this marketplace.

In Claude Code: `/plugin marketplace add ascend-so/plugins`, then `/plugin install ascend-so@ascend-so`.

## Use it

Type `/ascend`, then what you want:

- `/ascend https://www.instagram.com/reel/<code>/` breaks the Reel down: why it worked, its hook, how it is built.
- `/ascend transcript https://www.instagram.com/reel/<code>/` gives the transcript.
- `/ascend` with several Reel links says what they have in common.
- `/ascend what hooks are working in skincare right now`
- `/ascend how is @handle growing`
- `/ascend` on its own lists what you can ask.

In Claude Code and Cowork the command is written `/ascend:ascend`.

Ascend covers Instagram only.

## If the command doesn't show

- You are on a free Claude plan, or "Code execution and file creation" is off.
- Ascend isn't connected, or isn't switched on in this chat. Connect it on the plugin's Connectors tab, or open the + menu, choose Connectors, and switch Ascend on.
- The chat was opened before you added the plugin. Start a new one.
- You are on a Team or Enterprise plan and your workspace owner hasn't allowed members to add plugins.
- You added an older copy by uploading a zip. Remove it and add this one.

Without the command, the same words still work: ask Claude to "use Ascend" and say what you want.

## ChatGPT

ChatGPT has no slash commands for connected apps. Type `@Ascend` and then your question.
