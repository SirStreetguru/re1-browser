# RE1 Browser Edition

Resident Evil 1 (Classic REbirth) running in the browser via WebVM + Wine + CheerpX.

## How it works

1. A custom Dockerfile installs Wine + the game into a Debian i386 image
2. GitHub Actions builds an ext2 disk image from the Docker container
3. The disk image is deployed to GitHub Pages
4. CheerpX (WASM x86 JIT) runs the whole thing client-side in your browser

## Usage

Visit the deployed GitHub Pages URL and wait for the VM to boot.
Then run: `./launch.sh` to start the game.

## Credits

- [WebVM](https://github.com/leaningtech/webvm) by Leaning Technologies
- [CheerpX](https://cheerpx.io/) x86-to-WASM virtualization engine
- [Classic REbirth](https://classicrebirth.com/) by Gemini/Apple of Eden
- [Wine](https://www.winehq.org/) Windows compatibility layer
