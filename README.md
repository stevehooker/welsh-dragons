### welsh-dragons
# A Colab for ComfyUI and its manager with cloudflared
### Just some notes for CoLab Newbies, like myself...
https://github.com/stevehooker/welsh-dragons/blob/main/Comfyui_colab_with_manager.ipynb

I like to use a T4 with additional memory. That's 15Vram and 50ram. Lower ram will give OOM errors and force you into --HIGH_VRAM on startup. T4 with additional memory will start up with -- NORMAL_VRAM. Of course, this is slower than an A100 with 40vram, but cheaper. An A100 runs about 15 units/hour, my set-up at 2 units/hour. Of course, if you're just messing about you could not use a video card and that's really cheap while you set up your ComfyUI or something, then, terminate and "change run type" and Runtime > Run all to start a new session.

It takes, maybe, 10 minutes to check for updates and get back to your ComfyUI workspace under a new URL. But, once there, it's pretty good. Though occasionally your URL will break, or there'll be a bug in ComfyUI, or you'll add a new LoRA that means you need to restart that 10 minutes, again.

You'll definitely need Colab Pro, at least, as these days there is no free SD on Colab. You'll likely go up to Colab Pro Plus, as you'll be using it often. As well, you'll need to rise up from the Free Google Drive, as those checkpoints are heavy, and there are lots to have fun with.

I also have a ComfyUI install on my local machine, and I try to mirror it with Google Drive. And when I'm doing a lot of reading, watching YouTubes to learn ComfyUI and SD, it's much cheaper to mess around here, then go up to Google Colab.
