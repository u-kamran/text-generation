## Text Generation

Contains sample code from an educational session that I taught on the topic of Text Generation.

Builds and trains a Long Short-Term Memory (LSTM) machine learning model for generating text.

## Training Data

The Wonderful Wizard of Oz by Lyman Frank Baum - Downloaded from Project Gutenberg

| Version | Modifications |
| :-----: | :------------ | 
| v1 | Original Text |
| v2 | Empty Lines Removed |
| v3 | Chapter Titles Removed |
| v4 | Multiple Spaces Removed |
| v5 | Multiple Uppercase Letters Removed |
| v6 | Replaced Specific Unicode Characters |

The following Unicode characters were replaced:

| Character | Replacement |
| :-------: | :---------: | 
| `\u2014` | `-` |
| `\u2018` | `'` |
| `\u2019` | `'` |
| `\u201c` | `"` |
| `\u201d` | `"` |

## Training Results

The results from training the machine learning model are shown below:

**Figure 1 - Epochs 1 to 15**

![Epochs 1 to 15][figure-one]

**Figure 2 - Epochs 16 to 30**

![Epochs 16 to 30][figure-two]

**Figure 3 - Training Accuracy**

![Training Accuracy][figure-three]

[figure-one]: images/epochs-part-one.png "Epochs 1 to 15"
[figure-two]: images/epochs-part-two.png "Epochs 16 to 30"
[figure-three]: images/training-accuracy.png "Training Accuracy"

Examples of text generated by the model are shown below:

```
The scarecrow was now the ruler of the emerald city and although he was not a wizard the people were proud
```

```
The sun shone brightly as our friends turned their faces toward the land of the south they were all in the best of spirits and laughed and chatted together
```

## Model Weights

The saved model weights can be loaded as shown below:

```
model.load_weights('./weights/ckpt_30')
```

Note: the file `ckpt_30.data` will first need to be renamed to `ckpt_30.data-00000-of-00001`
