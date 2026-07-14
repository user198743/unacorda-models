# Una Corda model artifacts

Versioned, browser-ready piano transcription model artifacts used by
[Una Corda](https://github.com/user198743/unacorda).

## `model-v1`

- Asset: `note_pedal.fp16.onnx`
- SHA-256: `8f2533cc2b466e0b5cb41be22747ed3e3a0ab0dc80b3d11f9b4e7fccda043779`
- Size: 86,110,082 bytes
- Format: ONNX with float32 input/output and a mixed fp32/fp16 graph

The graph is derived from the public high-resolution piano transcription checkpoint
`CRNN_note_F1=0.9677_pedal_F1=0.9186.pth` published with Qiuqiang Kong et al.'s
*High-resolution Piano Transcription with Pedals by Regressing Onsets and Offsets Times*.
The original checkpoint is distributed through
[Zenodo record 4034264](https://zenodo.org/record/4034264), and the reference implementation
is archived at [bytedance/piano_transcription](https://github.com/bytedance/piano_transcription).

Release assets are immutable. A replacement graph is published under a new release tag rather
than overwriting an existing model. See `LICENSE` for this repository's terms; upstream components
retain their original licenses and attribution requirements.
