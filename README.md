This project implements a Transformer-based neural network to generate coherent and expressive music sequences in MIDI format. By leveraging the MAESTRO dataset, the model learns temporal dependencies and musical patterns, pushing the boundaries of AI-generated music.

Key Features:
  Dataset: The MAESTRO dataset is used, comprising over 1,200 hours of annotated piano performances. It includes precise timing and expressive dynamics, making it ideal for music generation tasks.
  
  Model Architecture:
      Embedding size: 256
      Number of Transformer layers: 4
      Attention heads: 8
      Vocabulary size: 307
      Adaptation of Transformer architecture for musical token sequences.
  
  Preprocessing:
      MIDI data tokenized into sequences of notes, velocities, and durations.
      Positional encodings are added to capture the temporal structure.
      
  Training:
      Framework: TensorFlow/Keras.
      Batch size: 64.
      Learning rate: 0.001.
      Epochs: 10.
      Loss Function: Sparse categorical cross-entropy.
      
  Music Generation:
      Starts with a seed sequence and predicts tokens iteratively.
      Techniques like top-k sampling and temperature scaling improve creativity and variability in the output.

      
Highlights:
    Generated Music: Produces diverse and rhythmically engaging MIDI files, capturing patterns from the training data.
    Evaluation:
        Quantitative: Validation loss plateaued, showing stable generalization.
        Qualitative: Demonstrates the ability to model long-term dependencies in music.
        
Applications:
AI tools for composers to inspire new creations.
Automated generation of background music for games, films, and more.
Music education and analysis tools.

How to Use:
Clone the repository.
Prepare the MAESTRO dataset and preprocess the MIDI files.
Train the Transformer model using the provided notebook.
Generate music by running the generation module with a seed sequence.
