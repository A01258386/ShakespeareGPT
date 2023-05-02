# ShakespeareGPT

**My Results**
ROMEO:
But you fret, hell, where Volivius:
They now I usless like, to to see this grand; I'll must sprinks dray-wretor upwon alond, liege wan thy lace blaniess to hanger and nour gruest:
Now to by betwers tot, tow, go:
Eve nor to his ghards wifill my join not.

LUCIY:
Lord,----
But thou sging them but
am they beens us
By thou sovore.

ISABELLA:
The pitsade but grove to hadgeles!

CLARD:
The kingle me; an your tords wants jecuntal.

MENVO:
I be e'll comfsir, whom in the sceed with mad him to is forgiving:
Go, be slouce ways! do to-smages:
Once it his susin, passess stond? the haspe, lew, ever some to me with dought:
In your hear him, and that, out thy whose my late all that you by joyly us beliess Lord:
Well-mone is not lets, for with!
He arre royper rivioled orcusion
What confess, temile you by that thou grurn that such differs I'll bear confetio-s:
To, no at and her long wornt, and on aflience;
And um you, profort, take, thou, names:
In mistragoing, now our beavehs exeny with.

GLOUCESTER:

HENRY Me, whose? but to good it that wing thy dukes,
I ward than war
offightant, I us onle adgrians viles.

PUMPERD:
It that advouter:
If ver have her.
Must now sow I wish that my brunk
But you renvenger am stand and of the loves mark own!
'Dacking to the sid, to? so.
Yet my singel I ranca: thou fult,
An king this woulds no the said out
offerds frul, I'll Rame, to beets nighm
in hims adughted diernm.
3 And Mow your whorth
And whom fetch unto will rest:
My brive, her his toward to that his sabired.
But, prewer, sorrow lom if curner,
But us so, tondury; wat's fastes for your heere whope snonet stand the father adviets Cappentriagh that brird
of say mover a desrick.

MONTAM:
You he; give
Nince, I is have.

Set:
BUCKINGHAM:
Let requmal I upon me.

HENRY BOLINGBRA:
That wife the back with wowitte,
Which bunnain fall more in in meept twate,
You staves that high pray plate on bring.

NORDUKE:
The stituly, maint, yet having. But, the castions:
O 'tis lace;--

BUCKINGS:
On; grave, before
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Shakespeare Language Modelling using GPT architecture
This repository contains an implementation of a language model based on the GPT architecture trained on the complete works of Shakespeare.

Overview
This notebook implements a transformer based language model using PyTorch. The model is trained on the complete works of Shakespeare in the input.txt file. After training, the model can be used to generate new text given a starting prompt.

Dependencies
PyTorch
Setup
To run this code, you will need to upload the input.txt file to the same directory as the notebook. You can find the input.txt file here: https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt

Model Architecture
The model consists of several Transformer blocks, each containing a Multi-Head Attention layer followed by a Feed-Forward layer. The final output layer is a linear layer followed by a softmax activation function. The model uses the Adam optimizer with a learning rate of 1e-3.

Hyperparameters
batch_size = 16
block_size = 32
max_iters = 5000
eval_interval = 100
learning_rate = 1e-3
device = 'cuda' if torch.cuda.is_available() else 'cpu'
eval_iters = 200
n_embd = 64
n_head = 4
n_layer = 4
dropout = 0.0
Training
The model is trained on the complete works of Shakespeare, split into a 90% training set and a 10% validation set. The model is trained for 5000 iterations with a batch size of 16.

Evaluation
The model is evaluated on the training and validation sets every 100 iterations using a batch size of 16. The loss is calculated using cross-entropy loss.

Output
After training, the model can be used to generate new text given a starting prompt. The model uses a temperature parameter to control the randomness of the generated text. A higher temperature value will result in more random text, while a lower temperature value will result in text that is more similar to the training data.







