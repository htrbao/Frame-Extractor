# Frame-Extractor

## 1. Prerequisites and System Requirements
- You must have [ffmpeg](https://ffmpeg.org) framework inside your system.
- Create 2 Folder `Videos` and `Keyframes`.

*You can freely choose the folder name, e.g. `My Very Detail Keyframes`, depending on how you want its name to appear on the bucket.*
			

## 2. Run
```
python3 extractor.py
```

- This will download `<video-name>.mp4` from the Bucket to `Videos` folder.
```
Videos
└──video-name.mp4
```
- Then extract the frame to `Keyframes/video-name/`
```
Keyframes
└── video-name
    ├── video-name_00xx.jpg
    ├── video-name_00xx.jpg
    ├── ...
    └── video-name_00xx.jpg
```

- Finally, it will upload the `Keyframes` folder back to the bucket.