```markdown
# Character-Level Text Generation using LSTM on Shakespeare's Text

This project implements a character-level text generation model using a Long Short-Term Memory (LSTM) network. The model is trained on a portion of Shakespeare's works and generates text that mimics the style of Shakespeare.

---

## 🚀 **Project Overview**
- **Goal:** Generate text character by character, predicting the next character in a sequence.
- **Data Source:** Shakespeare's complete works (downloaded from TensorFlow).
- **Model:** LSTM-based sequential model with a dense layer and softmax activation.
- **Training Data:** Sequences of 40 characters with a step size of 3.

---

## 📥 **Dependencies**
- Python 3.x
- TensorFlow
- NumPy

---




## 📝 **Model Details**
- **Input:** Sequence of 40 characters.
- **Output:** Probability distribution over the next character.
- **Architecture:**
  - LSTM Layer: 128 units
  - Dense Layer: Maps to the character space
  - Activation: Softmax

---

## 🎯 **Usage**
To generate text:
```python
print(generate_text(300, 0.5))
```
- `length`: Number of characters to generate.
- `temperature`: Controls randomness in prediction.

---

## 📊 **Results**
- Higher temperature → More diverse and creative text.
- Lower temperature → More conservative and predictable text.
