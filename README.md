### Song Creation AI with LSTM

This project aims to develop an innovative Song Creation Artificial Intelligence (AI) system using Long Short-Term Memory (LSTM) networks. By leveraging the power of deep learning and sequence modeling, our AI model is designed to compose original and compelling lyrics. The LSTM architecture enables the AI to capture intricate patterns and dependencies within music, allowing it to generate coherent and expressive compositions. Through this project, we hope to push the boundaries of music creation by combining human creativity with the capabilities of AI.

### Instructions for Setting up the Generator

These are the instructions for using the models. Because of the size of those models they could not be uploaded in here. The script to train them is in SongsText.ipynb.

Then, in that same file, execute:
```
model = keras.models.load_model('/path_to_model/song_lyrics_generator_Not_One.h5')
beginning = "Hi, my name is"
n_words = 300
complete_this_song(beginning, n_words)
```

## Some examples

With a model trained with only Snoop Dog songs, we get this results:
```
beginning = "Michael Jordan is"
n_words = 155
complete_this_song(beginning, n_words)
```
__"Michael Jordan is it done y girl free i'm just out in the world__

__you know you're love to you know__

__it's a secret in all and the sky i love found all my life__

__i've been afraid of me, i've been afraid by i've been tryna by you i've been thinking__

__i've been dreaming of you __

__i've been dreaming of you __

__i've been dreaming of you, dreaming of you, been dreaming of you__

__i've been dreaming of you, dreaming of you all of your life,__

__i've been dreaming of you __

__i've been dreaming of you __

__i've been dreaming of you, dreaming of you all my life,__

__i've been dreaming of you __

__i've been dreaming of you __

__i've been dreaming of you, dreaming of you all my life,__

__i've been dreaming of you __

__i've been dreaming of you __

__i've been dreaming of you, dreaming of you all my life,__

__i've been dreaming of you __

__i've been dreaming of"__

With the model trained with all songs we get:
```
beginning = "Is this love"
n_words = 300
complete_this_song(beginning, n_words)
```
__"Is this love you' h town__

__i'm coming in it with our love__

__i'm so good for my body__

__i know you for you all__

__that you must not the one to the left to the left__

__everything you want to the good of your heart__

__everything you were the one i hoped i was__

__just a way you a way you know how i saw the real you__

__thank god you blew it__

__thank god i dodged the bullet__

__i'm so over you so baby good lookin' out__

__i wanted you bad i'm so through with it__

__cuz honestly you turned out to be the best thing i never ha__

__and i'm gon' always be the best thing you never had__

__i bet it sucks to be you right now so sad you're hurt boo hoo__

__oh did you expect me to care__

__you don't deserve my tears__

__i guess that's why they ain't there__

__when i think that there was a time that i almost loved you__

__you showed you ass and i saw the real you__

__thank god you blew it__

__thank god i dodged the bullet__

__i'm so over you so baby good lookin' out__

__i wanted you bad"__

## Conclusions

The model is not the best thing in the internet right now. 

The verses are not really coherent, and we would need a metric apart from the model's accuracy to determine wether the phrases are well constructed or not. 

We are also not taking into account the rithm and the rhymes, very important in crating music.

In summary, we are not reinventing the wheel, trurn out this model can't compete with human imagination and inspiration.

## Next Steps

1. Perform objective evaluation: Use metrics like perplexity or BLEU score to assess the quality and coherence of generated lyrics compared to the original dataset. Additionally, gather human evaluators (professionals in the music industry) to rate the creativity, relevance, and fluency of the generated lyrics.
2. Apply diversity enhancement techniques: Combat repetitive patterns by experimenting with methods like Top-k sampling or Nucleus sampling to improve the diversity of generated lyrics.
3. Explore style transfer application: Investigate the implementation of style transfer techniques for song lyrics generation. For example, train the model on lyrics from a specific music genre and attempt to generate lyrics in a different genre while preserving the style of the original genre.
4. Scale up the model architecture: With increased computational resources, consider expanding the model's architecture to a wider and deeper structure. This can involve adding more layers or increasing the hidden units of the LSTM network, allowing the AI to capture more complex musical patterns and generate richer and more diverse song compositions.

## Authors

* **Andrés Canalejo Oliva**
* **Pablo Pérez González-Alberto**
* **Luis Zaldivar Lobato**




