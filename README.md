# IITISOCML17_project
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
    <h1>Type in Your Handwriting</h1>
    <h3>Intro For Our Model:</h3>
    <p>
        The instance has now arrived to drain out the shape of the miles of efforts and the counts of innumerous significant seconds to fabricate just few sheets of content in your customized handwriting.
      </p>
      <p>
        YES ! Typing in your own handwriting has now become easier as of never before and ever after !!
      </p>
      <p>
        The page you are viewing right now with the notion of curiosity and the sense of glad besides the matter of suspicion, is a part of our website, designed to generate the limitless text that you type in, in your personalized handwriting. 
      </p>
      <p>
        Our website is designed in the view of receiving the inputs of your desired content as the text and your customized handwriting as an image. 
      </p>
      <p>
        The latter phase comprises of the image generation of your input text in your preferred handwriting. The responsibility of this juncture is entirely carried out on the shoulders of the Machine Learning model, developed by our team with the virtue of VAE (Variational Auto-encoder) and GAN (Generative Adversarial Network) models. The overview of the techniques we followed to conceive this innovative Customized Type in your Handwriting model is disclosed in the following draft.
      </p>
      <p>
        Commencing with the speculation of auto-encoders to extract the strokes and the style vectors from the input image of the desired handwriting style, the task next to it holds the pre-processing of the image to the specific size- (224 x 224 px), while the desired content (text) after texting, is grasped as a string on the other hand. The extracted information is then dispatched into the GAN model to generate the image of the input content (text) in the inserted handwriting. Though the Generator of the GAN deals with generating such images, the final call to lay out the output is under the verdict of the Discriminator of the GAN. As acknowledged by a GAN disciple the discriminator delivers a bool on comparing the strokes of the handwriting in the image generated by the generator and the strokes of the authentic handwriting laid as the input reference. If the bool is not immediate to the desired accuracy, the next epoch is entertained to refine the image generated. Likewise, the model holds the deal of performing multiple epochs up to the extent of achieving the desirable contentment of the generated image in the view of the custom handwriting style and finally it steps out of the artificial model into the world of the livingly users as an output. 
      </p>
      <p>
        This exercise of assimilation and execution of the varied and modern techniques to develop such an innovative and handy model, could take shape through the collective and collaborative team work of our group involving:
      </p>
      <h3>Use the model on your own:</h3>
      <p>Clone the project in your project in your local machine. Using the terminal or command line interface, navigate to the project. Use the pip command<b>pip install -r requirements.txt</b> to download the required modules for the model.</p>
      <p>Using the command <b>python3 generate.py --image [path/to/image/in/local_machine] --message ["Provide a string to convert into your handwriting"]</b>. While passing the image try to pass the image which consists of a single line of your desired handwriting. Your output image will be saved to stati folder of this project.</p>
      <h3>Exploring the Web-Interface:</h3>
      <p>Navigate to the project using the terminal and run the following command.<b>uvicorn app:app --host 0.0.0.0 --port 8000</b>. Your website will be hosted locally in your machine and explore the web-interface.</p>
</body>
</html>
