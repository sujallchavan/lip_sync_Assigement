# Wav2Lip - Lip-Sync Model

This project generates realistic lip-sync videos from an image and an audio file using Wav2Lip.

## 📁 Project Structure

```
Wav2Lip/
├── checkpoints/               # Model weights directory
│    ├── face_sync.pth         # SyncNet model weight
│    └── wav2lip_gan.pth       # Wav2Lip GAN model weight
├── inputs/                    # Input media directory
│    ├── image.jpg             # Input face image
│    └── input_audio.mp3       # Input audio file
├── outputs/                   # Output media directory
│    └── result.mp4            # Lip-synced output video
├── inference.py               # Main script for inference
├── requirements.txt           # Python dependencies
└── ...                        # Other scripts
```

## 🛠️ Setup Instructions (Windows)

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/Wav2Lip.git
cd Wav2Lip
```

### 2. Create and Activate a Virtual Environment

```bash
python -m venv wav2lip_env
wav2lip_env\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Google Text-to-Speech (gTTS)

```bash
pip install gtts
```

### 4. Download Pre-trained Models

Place these files in the `checkpoints/` folder:

- [Download wav2lip_gan.pth](https://github.com/Rudrabha/Wav2Lip/releases/download/v1.0/wav2lip_gan.pth)
- [Download face_sync.pth](https://github.com/Rudrabha/Wav2Lip/releases/download/v1.0/face_sync.pth)

## ▶️ Run the Model

Make sure `inputs/image.jpg` and `inputs/input_audio.mp3` exist.

```bash
python inference.py --checkpoint_path checkpoints/wav2lip_gan.pth \
    --face inputs/image.jpg --audio inputs/input_audio.mp3 \
    --outfile outputs/result.mp4
```

### Output:

- `outputs/result.mp4`: Lip-synced video
#   l i p _ s y n c _ A s s i g e n m e n t _ Y u b i  
 "# lip_sync_Assigement" 
