# Awesome Video Understanding [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of APIs, open models, tools, datasets, and papers to search, analyze, and understand video.

Video understanding turns raw video into data that software and AI agents can use. This data includes transcripts, shots, scenes, objects, on-screen text, embeddings, and answers to questions. This list collects useful resources for each step. Each section is in alphabetical order.

## Contents

- [Video understanding APIs](#video-understanding-apis)
- [Open video-language models](#open-video-language-models)
- [Video encoders and embeddings](#video-encoders-and-embeddings)
- [Speech and audio](#speech-and-audio)
- [Shot and scene detection](#shot-and-scene-detection)
- [OCR in video](#ocr-in-video)
- [Object detection, segmentation, and tracking](#object-detection-segmentation-and-tracking)
- [Tools and libraries](#tools-and-libraries)
- [MCP servers for video](#mcp-servers-for-video)
- [Datasets and benchmarks](#datasets-and-benchmarks)
- [Surveys and papers](#surveys-and-papers)
- [Related](#related)

## Video understanding APIs

Hosted services that analyze video for you.

- [Amazon Bedrock Data Automation](https://aws.amazon.com/bedrock/bda/) - Managed service that turns video, audio, images, and documents into structured insights.
- [Amazon Nova](https://docs.aws.amazon.com/nova/latest/userguide/modalities-video.html) - Video input for Amazon Nova understanding models on Amazon Bedrock.
- [Amazon Rekognition Video](https://docs.aws.amazon.com/rekognition/latest/dg/video.html) - Detects labels, faces, people, text, and segments in stored and streaming video.
- [Azure AI Video Indexer](https://learn.microsoft.com/en-us/azure/azure-video-indexer/video-indexer-overview) - Extracts transcripts, faces, OCR, labels, shots, and scenes in the cloud or at the edge with Azure Arc.
- [Cloudglue](https://www.cloudglue.dev/) - APIs that turn video into context for AI, including speech, diarization, and visual descriptions.
- [Gemini API video understanding](https://ai.google.dev/gemini-api/docs/video-understanding) - Send video to Gemini models to describe, transcribe, and answer questions about it.
- [Google Cloud Video Intelligence API](https://cloud.google.com/video-intelligence) - Pretrained models for labels, shot changes, object tracking, text, and explicit content.
- [Google Vertex AI video understanding](https://cloud.google.com/vertex-ai/generative-ai/docs/multimodal/video-understanding) - Video input for Gemini models on Google Cloud.
- [Memories.ai](https://memories.ai/) - Video intelligence platform for search, summarization, and multimodal understanding.
- [Mixpeek](https://mixpeek.com/) - Turns video, images, audio, and documents into data that software can search and classify.
- [OpenAI Cookbook video example](https://cookbook.openai.com/examples/gpt_with_vision_for_video_understanding) - Sends sampled video frames to GPT models to describe and narrate a video.
- [TwelveLabs](https://docs.twelvelabs.io/) - Video foundation models, Marengo and Pegasus, with APIs for search, embeddings, and text generation.
- [TwelveLabs in Amazon Bedrock](https://aws.amazon.com/bedrock/twelvelabs/) - TwelveLabs video models available through Amazon Bedrock.
- [Video Context](https://videocontextapi.com) - Model-agnostic video context API for apps and AI agents. In private beta.
- [VideoDB](https://videodb.io/) - Video data infrastructure for ingestion, machine annotation, and retrieval.

## Open video-language models

Models with open weights that take video as input and produce text.

- [Ask-Anything (VideoChat)](https://github.com/OpenGVLab/Ask-Anything) - Chat-centric video understanding models and the MVBench benchmark.
- [Cosmos-Reason1](https://github.com/nvidia-cosmos/cosmos-reason1) - NVIDIA models that reason about physical common sense in video.
- [InternVL](https://github.com/OpenGVLab/InternVL) - Open multimodal LLM family with image and video input.
- [LLaVA-NeXT](https://github.com/LLaVA-VL/LLaVA-NeXT) - Code and models for LLaVA-OneVision and LLaVA-Video.
- [MiniCPM-V](https://github.com/OpenBMB/MiniCPM-V) - Small multimodal LLMs for image and video understanding on devices.
- [Perception Models](https://github.com/facebookresearch/perception_models) - Meta Perception Encoder and Perception Language Model for image and video.
- [Qwen3-VL](https://github.com/QwenLM/Qwen3-VL) - Qwen vision-language models with video input. The repo also covers Qwen2.5-VL.
- [Tarsier](https://github.com/bytedance/tarsier) - Video-language models for detailed video description.
- [Video-ChatGPT](https://github.com/mbzuai-oryx/Video-ChatGPT) - Video conversation model with a benchmark for video chat models.
- [Video-LLaVA](https://github.com/PKU-YuanGroup/Video-LLaVA) - Aligns image and video features before projection into an LLM.
- [VideoChat-Flash](https://github.com/OpenGVLab/VideoChat-Flash) - Hierarchical compression for long-context video modeling.
- [VideoLLaMA 2](https://github.com/DAMO-NLP-SG/VideoLLaMA2) - Video LLM with spatial-temporal modeling and audio understanding.
- [VideoLLaMA 3](https://github.com/DAMO-NLP-SG/VideoLLaMA3) - Multimodal foundation models for image and video understanding.

## Video encoders and embeddings

Models that turn video into vectors for search, retrieval, and classification.

- [Amazon Nova Multimodal Embeddings](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) - One embedding space for text, documents, images, video, and audio.
- [CLIP](https://github.com/openai/CLIP) - Contrastive image-text model, often applied to sampled video frames.
- [CLIP4Clip](https://github.com/ArrowLuo/CLIP4Clip) - CLIP-based model for text-to-video retrieval.
- [InternVideo](https://github.com/OpenGVLab/InternVideo) - Video foundation models, including InternVideo2, for recognition, retrieval, and video-text tasks.
- [LanguageBind](https://github.com/PKU-YuanGroup/LanguageBind) - Aligns video, audio, depth, and infrared to language in one embedding space.
- [OpenCLIP](https://github.com/mlfoundations/open_clip) - Open source implementation of CLIP with many pretrained weights.
- [TwelveLabs Marengo](https://docs.twelvelabs.io/docs/concepts/models/marengo) - Multimodal embedding model for video search and retrieval.
- [V-JEPA 2](https://github.com/facebookresearch/vjepa2) - Self-supervised video encoder from Meta.
- [Vertex AI multimodal embeddings](https://cloud.google.com/vertex-ai/generative-ai/docs/embeddings/get-multimodal-embeddings) - Embeddings for text, images, and video on Google Cloud.
- [VideoMAE](https://github.com/MCG-NJU/VideoMAE) - Masked autoencoders for self-supervised video pretraining.
- [VideoPrism](https://github.com/google-deepmind/videoprism) - Google DeepMind foundational visual encoder for video understanding.
- [X-CLIP](https://huggingface.co/docs/transformers/model_doc/xclip) - Video-text model that extends CLIP, available in Hugging Face Transformers.

## Speech and audio

Transcription, speaker diarization, and voice activity detection.

- [faster-whisper](https://github.com/SYSTRAN/faster-whisper) - Fast Whisper inference with CTranslate2.
- [Parakeet TDT 0.6B v3](https://huggingface.co/nvidia/parakeet-tdt-0.6b-v3) - NVIDIA speech recognition model for 25 European languages.
- [pyannote.audio](https://github.com/pyannote/pyannote-audio) - Speaker diarization toolkit with pretrained pipelines.
- [Silero VAD](https://github.com/snakers4/silero-vad) - Small pretrained voice activity detector.
- [Whisper](https://github.com/openai/whisper) - OpenAI general-purpose speech recognition model.
- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) - Whisper in C/C++ for local inference on CPU and GPU.
- [WhisperX](https://github.com/m-bain/whisperX) - Whisper with word-level timestamps and speaker diarization.

## Shot and scene detection

Find cuts, transitions, and keyframes.

- [AutoShot](https://github.com/wentaozhu/AutoShot) - Shot boundary detection model and short video dataset.
- [FFmpeg scdet filter](https://ffmpeg.org/ffmpeg-filters.html#scdet) - Built-in FFmpeg filter that detects scene changes.
- [FFmpeg select filter](https://ffmpeg.org/ffmpeg-filters.html#select) - Selects frames by scene change score, for example `select='gt(scene,0.4)'`.
- [PySceneDetect](https://github.com/Breakthrough/PySceneDetect) - Python and OpenCV tool and library for scene cut and transition detection.
- [TransNetV2](https://github.com/soCzech/TransNetV2) - Neural network for shot boundary detection.

## OCR in video

Read on-screen text, captions, and burned-in subtitles.

- [docTR](https://github.com/mindee/doctr) - Deep learning library for text detection and recognition.
- [EasyOCR](https://github.com/JaidedAI/EasyOCR) - Ready-to-use OCR for 80+ languages.
- [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR) - OCR toolkit for images and documents with support for 100+ languages.
- [Tesseract](https://github.com/tesseract-ocr/tesseract) - Open source OCR engine.
- [VideOCR](https://github.com/timminator/VideOCR) - Extracts hardcoded subtitles from video with a GUI.

## Object detection, segmentation, and tracking

Find and follow objects, people, and points across frames.

- [BoxMOT](https://github.com/mikel-brostrom/boxmot) - Pluggable multi-object tracking modules for detection models.
- [ByteTrack](https://github.com/FoundationVision/ByteTrack) - Multi-object tracking that associates every detection box.
- [CoTracker](https://github.com/facebookresearch/co-tracker) - Model that tracks any point across a video.
- [Grounded SAM 2](https://github.com/IDEA-Research/Grounded-SAM-2) - Detects, segments, and tracks objects in video from text prompts.
- [SAM 2](https://github.com/facebookresearch/sam2) - Meta Segment Anything Model 2 for promptable segmentation in images and video.
- [SAM 3](https://github.com/facebookresearch/sam3) - Meta Segment Anything Model 3 for segmentation from text and visual prompts.
- [Supervision](https://github.com/roboflow/supervision) - Reusable computer vision tools for detection, tracking, and annotation.
- [Ultralytics YOLO](https://github.com/ultralytics/ultralytics) - YOLO models for detection, segmentation, pose, and tracking.

## Tools and libraries

Decode, load, process, and build video pipelines.

- [decord](https://github.com/dmlc/decord) - Efficient video loader for deep learning.
- [FFmpeg](https://ffmpeg.org/) - Complete toolkit to record, convert, and stream audio and video.
- [Mediabunny](https://github.com/Vanilagy/mediabunny) - TypeScript toolkit to read, write, and convert media files in the browser.
- [MMAction2](https://github.com/open-mmlab/mmaction2) - OpenMMLab toolbox for action recognition and video understanding.
- [NVIDIA Video Search and Summarization](https://github.com/NVIDIA-AI-Blueprints/video-search-and-summarization) - Reference architecture for video analytics agents with VLMs and RAG.
- [OpenCV](https://github.com/opencv/opencv) - Computer vision library with video capture and processing.
- [PyAV](https://github.com/PyAV-Org/PyAV) - Python bindings for the FFmpeg libraries.
- [PySlowFast](https://github.com/facebookresearch/SlowFast) - Meta codebase for video classification models such as SlowFast.
- [TorchCodec](https://github.com/meta-pytorch/torchcodec) - Video and audio decoding for PyTorch on CPU and GPU.
- [torchvision video](https://docs.pytorch.org/vision/stable/io.html) - Video read and write functions in torchvision.
- [yt-dlp](https://github.com/yt-dlp/yt-dlp) - Command-line audio and video downloader.

## MCP servers for video

[Model Context Protocol](https://modelcontextprotocol.io) servers that give AI agents video tools.

- [ffmpeg-mcp](https://github.com/video-creator/ffmpeg-mcp) - MCP server that uses the FFmpeg command line to search, clip, and concatenate local video.
- [mcp-server-youtube-transcript](https://github.com/kimtaeyoon83/mcp-server-youtube-transcript) - MCP server that downloads YouTube video transcripts.
- [mcp-video-analyzer](https://github.com/guimatheus92/mcp-video-analyzer) - MCP server that turns video into transcripts, keyframes, OCR text, and metadata.
- [Mixpeek MCP server](https://github.com/mixpeek/mcp-server) - MCP server for the Mixpeek API.
- [TwelveLabs MCP server](https://docs.twelvelabs.io/docs/advanced/model-context-protocol) - MCP server for TwelveLabs video search and analysis.
- [VideoDB Agent Toolkit](https://github.com/video-db/agent-toolkit) - VideoDB context and MCP server for AI agents and IDEs.

## Datasets and benchmarks

### Datasets

- [ActivityNet](http://activity-net.org/) - Large-scale benchmark for human activity understanding.
- [Charades-STA](https://github.com/jiyanggao/TALL) - Temporal grounding of sentences in Charades videos.
- [Ego4D](https://ego4d-data.org/) - Large egocentric video dataset with benchmarks.
- [HowTo100M](https://www.di.ens.fr/willow/research/howto100m/) - Narrated instructional videos for video-text learning.
- [Kinetics](https://arxiv.org/abs/1705.06950) - Human action video dataset from YouTube clips.
- [MSR-VTT](https://www.microsoft.com/en-us/research/publication/msr-vtt-a-large-video-description-dataset-for-bridging-video-and-language/) - Video description dataset for video captioning and retrieval.
- [Panda-70M](https://github.com/snap-research/Panda-70M) - 70M video clips with captions from multiple cross-modality teachers.
- [QVHighlights](https://github.com/jayleicn/moment_detr) - Moment retrieval and highlight detection from natural language queries.
- [Something-Something V2](https://www.qualcomm.com/developer/software/something-something-v-2-dataset) - Labeled clips of people who do basic actions with everyday objects.

### Benchmarks

- [EgoSchema](https://egoschema.github.io/) - Long-form video question answering on egocentric video.
- [LongVideoBench](https://github.com/longvideobench/LongVideoBench) - Benchmark for long-context interleaved video-language understanding.
- [LVBench](https://github.com/zai-org/LVBench) - Benchmark for extreme long video understanding.
- [MLVU](https://github.com/JUNJIE99/MLVU) - Multi-task long video understanding benchmark.
- [MVBench](https://huggingface.co/datasets/OpenGVLab/MVBench) - Multi-modal video understanding benchmark with 20 temporal tasks.
- [Perception Test](https://github.com/google-deepmind/perception_test) - Google DeepMind benchmark for perception skills of multimodal models.
- [Video-MME](https://github.com/MME-Benchmarks/Video-MME) - Evaluation benchmark for multimodal LLMs in video analysis.

### Evaluation toolkits

- [lmms-eval](https://github.com/EvolvingLMMs-Lab/lmms-eval) - Evaluation toolkit for multimodal models across text, image, video, and audio.
- [VLMEvalKit](https://github.com/open-compass/VLMEvalKit) - Evaluation toolkit for large vision-language models.

## Surveys and papers

- [A Comprehensive Study of Deep Video Action Recognition](https://arxiv.org/abs/2012.06567) - Survey of deep learning methods for video action recognition.
- [Awesome-LLMs-for-Video-Understanding](https://github.com/yunlong10/Awesome-LLMs-for-Video-Understanding) - Paper list that goes with the Vid-LLMs survey.
- [Self-Supervised Learning for Videos: A Survey](https://arxiv.org/abs/2207.00419) - Survey of self-supervised video representation learning.
- [Video-Language Understanding: A Survey](https://arxiv.org/abs/2406.05615) - Survey from model architecture, model training, and data perspectives.
- [Video Transformers: A Survey](https://arxiv.org/abs/2201.05991) - Survey of transformer models for video.
- [Video Understanding with Large Language Models: A Survey](https://arxiv.org/abs/2312.17432) - Survey of video LLMs (Vid-LLMs).

## Related

- [video-schema](https://github.com/video-context/video-schema) - Open JSON schema for video data.
- [video-tools-mcp](https://github.com/video-context/video-tools-mcp) - MCP server with local FFmpeg video tools.

## Contributing

Contributions are welcome. Read the [contribution guidelines](CONTRIBUTING.md) first.

---

Maintained by [Video Context](https://videocontextapi.com).

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors waived all copyright and related or neighboring rights to this work. See [LICENSE](LICENSE).
