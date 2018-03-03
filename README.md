# Character Level Text Generation

For this exercise we will be generating text with the same writing style as the writer, the LSTM model has been trained from. This model will be trained in the charater-level which means that the sentence: 
>**"The quick brown fox jumps over the lazy dog."**

has a total of:

```python
sentence = list("The quick brown fox jumps over the lazy dog.")
print(sentence)
>>>> ['T','h','e',' ','q','u','i','c','k',' ','b','r','o','w','n',' ','f', 'o','x',' ','j','u','m','p','s',' ','o', 'v','e', 'r',' ','t','h','e',' ','l','a','z','y',' ','d','o','g','.']
len(sentence)
>>>> 44
```
44 variables

The model will be fed a certain amount of character and it will try to predict the next character as seen below:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<i>The quick brown fox jumps over the lazy do </i>**[?]**

The model should predict the letter **"g"**


The model will not be case sensitive and it will not ignore punctuations. It will not read words but specific letters.It will also need an initial input phrase of 40 characters in order to generate text and from there its output will become its input.

## Sample Generation

### Shakespeare
***One epoch***

chus:
my lord, i hear.

pericles:
most him and the beging of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of my bear the bear of

***Three epochs***

lucentio:
what shall i was the world that i will be so life
the man in the shall be the such a threel.

benedick:
what shall i lies the ways that well be so soul.

cornwall:
i will not be not the world of thy loved,
that i am the strength of the hands of the good
that i will be the arm of the hands and soul.

king richard ii:
hark the sun and

