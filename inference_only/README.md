# Minimal VITS Inference Package

This directory contains a stripped-down set of files for running
`cmd_inference.py` to synthesize speech with a pre-trained VITS model.
Only the runtime dependencies and model code required for inference are
included.

## Usage

1. Install Python 3.8 and the packages in `requirements.txt`.
2. Provide a trained model checkpoint and configuration file.
3. Run the command:
   ```bash
   python -m inference_only.cmd_inference -m G_0.pth -c config.json \
       -o output_dir -l 日本語 -t "こんにちは" -s SpeakerName
   ```

See `cmd_inference.py` for all command line options.
