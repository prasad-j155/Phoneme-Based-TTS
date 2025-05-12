# Phoneme-Based-TTS

🔧 Model Used and Why
We used the Kokoro TTS model (hexgrad/Kokoro-82M). It is a small and fast text-to-speech model. We chose it because:

It gives good-quality speech

It works quickly and doesn’t need much memory

It is easy to use in code

👉 Note:
You don’t need to convert text to phonemes manually. Kokoro model does this inside itself. You can give normal text, and it will automatically turn it into phonemes before generating speech.

🧪 How We Tested It
We checked how close the generated audio is to the real audio using:

L1 Loss: Checks how much the generated and original sounds differ.

L2 Loss: Similar to L1, but gives more weight to bigger mistakes.



🎯 What We Observed
Kokoro gave clear and smooth audio from text.

The L1 and L2 scores showed the generated audio was close to the original.

Since Kokoro converts text to phonemes itself, we didn’t need extra steps.

I have uploaded a streamlit app using same model : 

🚀 What Can Be Improved
Add other testing methods like KL Divergence or DTW.

Try different voice styles from Kokoro.

In the future, we can give phonemes directly for more control.