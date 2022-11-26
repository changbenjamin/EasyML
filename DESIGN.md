### My Name

Benjamin Chang

### Project Name

EasyML

### Project Design Overview

There were many different parts to this project that had to all be integrated together in a cohesive website. First, there were the machine learning algorithms, which were mostly written by ML researchers in Python, but had to be edited for the website. Next, there was the web application, which used Python and allowed the algorithms to be run on the website. Lastly, there was the actual website, which was written in HTML and CSS. I will walk through the design of this project in chronological order of how I implemented it.

# Machine Learning Algorithm Design

First, I had to find and connect relevant machine learning algorithms for this website. I initially wanted to use the AlphaFold protein folding algorithm in order to take in an input amino acid sequence and show an image of the folded protein. I ran into multiple issues with this code, such as the program taking 10-15 minutes to run and the web app not showing pictures properly.

Instead, I decided to go with a similar but more manageable part of the protein algorithm, which takes in an amino acid sequence and classifies it into one of many different protein types. Connecting this code to the website took the large majority of my time in this project. The machine learning algorithm was extremely convoluted and it was designed for batch file inputs, not single amino acid sequences. I had to code a completely new input program which took in a single amino acid sequence as a string and treated it like a list, transformed it into a float, and then run it through the model. Changing the number of features of the model finally got it to work with this system.

During the frustration with this protein algorithm, I planned to change the model to a simple algorithm to classify images to dogs or cats. This implementation was much easier to connect to the website, as it was already created with a web application in mind, so I had to connect to my web application, but the body of the code was mostly unchanged. The code for both of these algorithms were found on Kaggle.

After I got the protein algorithm to work, I thought it would be best to include both of these algorithms on the website. I think that having both algorithms actually significantly improved the project, as it can be used as a platform to add more ML programs in the future.

# Web Application Design

After finishing the code for the machine learning algorithms, I had to find a way to present those algorithms in a user-friendly way on the website. I had originally planned to run the Python code on the website itself, but I learned that there were web applications that would streamline that process to improve the UI/UX of the code.

I chose to use the web application called Anvil, as it was Python-based and was free. On Anvil, I created the user interface for both of the web apps, which connected directly to my machine learning algorithms (which were running on my Deepnote notebook). The Anvil code was written in Python and took in the input string/file, sent it to the Deepnote notebook, and returned the algorithms' output.

I embedded Anvil to my website through an HTML code block.

# Website Design

Initially, I designed the HTML and CSS for my website completely by myself, using parts of code from my homework and other projects. The website had a homepage, which connected to pages for the other two programs, Protein Classifier and Pet Classifier.

However, as Angela can attest to, my website design skills are pretty bad. My roommate laughed at my website when he saw it and recommended me to use a platform called nicepage.com to help me design the website, which helped a lot. I adapted my HTML and CSS code to their HTML template and CSS files, which helped with the aesthetics significantly.

### Final Design Thoughts

I did not expect my project to turn out the way it did, but I'm really happy about it! I thought that pivoting from a protein-folding website to a general machine learning platform website was a much better idea. Although the machine learning algorithms were harder to implement than initially expected, I was able to use what I'm learning in my ML course to do so, which was a great way to see the applications of my coursework.

I hope that you enjoy the website as well!