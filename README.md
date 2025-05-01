# Typo Workshop: Your Personal AI Typo Corrector

**Project Background**  
Every time I write emails, assignments, or blog posts, my brain thinks one thing but my fingers type something completely different—endless typos that disrupt my flow and waste my time. To solve this, I created a personalized AI assistant that automatically detects and corrects my typos in real time.

**Key Features**  
1. **Efficient Fine-Tuning**: Uses Flan-T5 with QLoRA to learn your unique typo patterns.  
2. **End-to-End Pipeline**: Data Collection → Model Training → Evaluation → Gradio Demo.  
3. **Low Memory Footprint**: 4-bit quantized model runs smoothly on GPUs with 8–16 GB VRAM.  
4. **One-Click Scripts**: Easy-to-use command-line interfaces for training and inference.


**Quick Start**  
```bash
git clone --recurse-submodules https://github.com/Tzara911/typo-workshop.git
cd typo-workshop
pip install -r requirements.txt
python src/train.py --data_path data/typo_dataset.jsonl
python src/predict.py --text "waht is your name?"

