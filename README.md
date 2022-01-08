### Hi there 👋
My name is Luca and I'm currently working on a custom CRM to enable recommendation based on a Deep Contextual Multi-Armed Bandits algorithm.
In the past I used to work a lot with images, automated processes and OCRs. 
In order to solve some of the problems I tackled, I had to create or fork a couple repos that you can find here. In particular:

### [Shutter](https://github.com/Rainelz/shutter)
My first side project, that then became my python playground to test some programming approaches. 

It started as a tool to benchmark image preprocessing algorithms against OCR implementations.

Needs changed over time and eventually became a tool to generate document images to train deep learning models. 

I used it to pretrain models with different architectures and then finetune on the actual problem I had with a limited dataset. 

I successfully trained a classifier for documents and a Super Resolution GAN to improve image scans, I was planning to train a detector and a custom OCR as well but priorities have changed.

### [EfficientNet-PyTorch](https://github.com/Rainelz/EfficientNet-PyTorch)
Forked the original repo a while ago and modified it to be trained on single channel grayscale images; nothing special but worked like a charm (94,5% acc on rvl-cdip) / (98% acc on my classification problem)

### [Doc-SR](https://github.com/Rainelz/Doc-SR)
More or less same story here. I had a lot of images to pass to an OCR algorithm that failed to produce a consistent result due to poor quality of the scans... Eventually ended up with this fork which I used to train a super resolution GAN to mainly do 3 things:

- Denoise Image
- Invert White on black text
- Generate a super resolved version of the original

Results were pretty neat and granted me up to 500% accuracy gain on OCR tasks that were hard failing without this preprocessing.
It was all about generating the right images with [shutter](#shutter) and add the right loss functions.

Check [this result](https://imgsli.com/MTY1MjE)

### [Botox](https://github.com/Rainelz/botox)
Maybe the coolest one, a Mac OS tray app thought to easily insert your username and password every time you need to (I used to do it 8/10 times a day!).
It can be invoked from the touchbar (Quick Action) or with a keyboard shortcut.

The credentials are kept encrypted and decrypted only inside the stack of the functions doing the typing job. 

100% secure? maybe not. Handful? definetely. Say goodbye to keychain access popup or login screens.  

## Contact
`'@'.join(['lucaranalli7', 'gmail.com'])`
