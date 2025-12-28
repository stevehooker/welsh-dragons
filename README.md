# Welsh Dragons

Museum-quality Welsh dragon art for your home or business.

## ComfyUI Colab Notebook

A streamlined Google Colab notebook for running ComfyUI with persistent storage and easy setup.

### Features

- **Persistent Google Drive Storage**: All your work is saved to `/content/drive/MyDrive/ComfyUI`
- **ComfyUI Manager Support**: Easy custom node management (optional)
- **Cloudflare Tunnel**: Secure external access to your ComfyUI instance
- **Optimised Defaults**: Fast startup with minimal updates
- **Modular Setup**: Five clear sections for easy troubleshooting

### Quick Start

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stevehooker/welsh-dragons/blob/main/notebooks/comfyui_colab_with_manager.ipynb)

1. Click the "Open in Colab" badge above
2. Run Section 1 to mount Google Drive
3. Run Section 2 to install/update ComfyUI
4. Run Section 3 to install dependencies (required each session)
5. Run Section 4 to install ComfyUI Manager (optional, disabled by default)
6. Run Section 5 to start ComfyUI and get your access URL

### Important Notes

- **No Checkpoints Included**: This notebook provides a clean ComfyUI installation without any pre-installed models or checkpoints
- **Google Drive Location**: Your ComfyUI installation lives at `/content/drive/MyDrive/ComfyUI`
- **Add Your Own Content**: Upload custom nodes to `/content/drive/MyDrive/ComfyUI/custom_nodes/`
- **Add Checkpoints**: Upload models to `/content/drive/MyDrive/ComfyUI/models/checkpoints/`
- **Dependencies Required**: Python packages must be reinstalled each new Colab session (automated in Section 3)
- **Persistent Storage**: ComfyUI, custom nodes, and models persist across sessions when using Google Drive

### Default Settings

The notebook is optimised for quick startup on subsequent runs:

- ✅ **Mount Google Drive**: Enabled (saves your work)
- ☐ **Update ComfyUI**: Disabled (only enable when you want updates)
- ✅ **Install Dependencies**: Enabled (required each session)
- ☐ **Install ComfyUI Manager**: Disabled (skip after first setup)
- ☐ **Install Custom Node Dependencies**: Disabled (skip after first setup)

### Typical Workflow

**First Time Setup** (15-20 minutes):
1. Run all sections with defaults
2. Enable ComfyUI Manager in Section 4 if desired
3. Upload your checkpoints to Google Drive

**Subsequent Sessions** (5-7 minutes):
1. Mount Google Drive (Section 1)
2. Skip ComfyUI update (Section 2 - already unchecked)
3. Install dependencies (Section 3 - runs automatically)
4. Skip Manager update (Section 4 - already unchecked)
5. Start ComfyUI (Section 5)

### Customisation

All options are controlled via checkboxes in form-style cells:

- **Google Drive**: Save to Drive or use temporary Colab storage
- **ComfyUI Updates**: Pull latest changes from GitHub
- **Dependencies**: Install/skip Python packages
- **ComfyUI Manager**: Install/update the Manager extension
- **Custom Nodes**: Install dependencies for your custom nodes

### Technical Details

- **GPU**: Tesla T4 (15GB VRAM)
- **Python**: 3.12.12
- **PyTorch**: 2.9.0+cu126 (CUDA 12.1)
- **Access**: Cloudflared tunnel (public URL)
- **Storage**: Google Drive (persistent) or Colab temp (ephemeral)

### Troubleshooting

**"ModuleNotFoundError"**: Ensure Section 3 (Install Dependencies) is checked and has run successfully.

**"Can't find main.py"**: Make sure Section 2 completed successfully and you're in the correct workspace directory.

**"Connection refused"**: Wait a few seconds for the cloudflared tunnel to establish, then refresh the URL.

### Contributing

Issues and pull requests welcome at [github.com/stevehooker/welsh-dragons](https://github.com/stevehooker/welsh-dragons)

### Licence

ComfyUI is created by [comfyanonymous](https://github.com/comfyanonymous/ComfyUI). This notebook is a convenience wrapper for easy Colab deployment.