# sd-webui-embeddings-queue-helper
Helpful to test different embeddings in one go (added to **positive prompt** only)

This is another fork of **Yinzo's Lora-queue-helper**, but for embeddings instead of loras. https://github.com/Yinzo/sd-webui-Lora-queue-helper

As I already have one fork of Yinzo's Lora-queue-helper, I can't make another. Hence this new repository.

Works even when using embeddings via symbolic links on Automatic1111.

Only tested on my Linux Mint system. Not tested on Windows or Mac.

I don't really know Python, so I enlisted some help from Claude 3.5 Sonnet. Basically this is Claude's rewrite of Yinzo's Lora-queue-helper (or of my fork, but that's also Claude's work, mostly).

## Install
To install from webui, go to Extensions -> Install from URL, paste https://github.com/rar0n/sd-webui-embeddings-queue-helper into the URL field, and press Install.
Then go to Extensions -> Installed tab, Press "Apply and restart UI".

## How to use
1. Locate the **Script** drop-down menu in the bottom left corner of Automatic1111 web UI
2. Select **Queue selected Embeddings (batch)**
3. Under **Select Directory** select the folders containing the Embeddings you want to use (Or click **All**)
   + I suggest to use **Use Custom Embeddings path** (Depending how many embeddings you have or your folder structure)
       + Paste in your folder path of the category of Embedding(s) you want to test / use
4. Under **Embeddings** select the Embedding(s)'s you want to test (or click **All**)
   + At least one Embeddings folder has to be selected first for the Embeddings section to show up.
   + If you've got a lot of folders, you have to scroll down past the **Select Directory** section to reach it
5. **Generate!**

## Tips

- Place your Embeddings into **sub-folders** by category (like "tools", "characters", or some such).
- This version only applies embeddings to the **positive prompt**.
- For applying to the negative prompt use this version: https://github.com/rar0n/sd-webui-negative-embeddings-queue-helper
