# Stuffing you Code with Pillow: An extremely beginners guide to Image Sourcery in Python
### And why I dumped the pytz and bokeh story for a Pillow one

---

After an emotional breakdown trying to figure out what ‘pytz’ actually wants from me and nearly getting dumped by Bokeh and its overly flamboyant charts and graph as if i was at the London Pride, I decided to spend my weekend in the company of something softer: Pillow. Yes, Pillow; literally and figuratively — literally as in bed and of course figuratively as in Python’s favorite library for image processing; not a sleep aid or adult hotline.

---

# Stuffing your code with Pillow: A peculiar beginners' Guide to Image Sorcery in Python 



This story is for all of you out there, just like myself, desperately trying to self-learn programming. The process goes like this; 

1. You start by never knowing where to start. 
2. To me I start looking at GIT tutorials as I consider Git is the foundation of good practices in collaborative projects.
3.  Go to your best friend google search, or your other profile on [dev.to](https://www.dev.to) do some research and voila; you **initiate** your quest to learning *Git* - *see what I've done there?* 
4. Five hours later you find yourself deep in the Docs of React and wondering how did you end up in the docs of a framework I didn't know exist - remember my experience with programming is at the extreme end of the beginner level. forget about libraries, pythons, frameworks and dragons. Pillow is as simple as this: Do you want to crop your ex face out of a photo programmatically? Then you need Pillow. Not Adobe. PILLOW.

## But what is Pillow you may ask -

As I said above, let's not name names; who cares if it's a library, Python or traditional. I am aiming to lay it down just how I have it in my head. And then I will give you some real-world use cases of the Marshmallow Assassin, as given on its [Pillow's official website](https://pillow.readthedocs.io/en/stable/). For now though, here is my computer illiterate explanation of the thing.

## Fun Pillow Fact

> *"Legend has it that Pillow was created by a Pythonista who got tired of opening Photoshop just to resize memes."*

No not really, I totally made that up for my own amusement just because I wanted to use the Pythonista here. 

## Let my unorthodox, twisted Pillow tutorial begin -

Your steps to creating your own 90's Adobe Photoshop

```bash
pip install pillow
```

Yes. Your *pi*p* will install pillow somewhere in the ?motherboard? Just go with it. For this little story the above line of code installs a library that can literally open an image of a cat and turn it into grayscale sadness. For this story, I am using a screenshot of my search on Git Tutorials. And one last tip I keep on seeing everywhere:

> #### When installing libraries from pip, there's apparently something tragic about to happen down the line (which I never reach), if you install globally. So do the virtual environment process for a project just as common (?) good practice before installing libraries

```python
from PIL import Image

image = Image.open('your-own-project.jpg')
image.show()
#Just make sure you got one off the world wide web
```

Now! These three lines and the Marshmallow Assassin becomes your personal gallery curator. Although, fair warning: if image.show() opens your system’s default viewer and if that's Microsoft Paint, |'d suggest leaving Pillow for now, open the balcony door and throw your machine away; you have other problems to solve. 😁

Below are my interpretations of the range of image processing provided to you by the Pillow

#### Resizing

```python
small = image.resize((100, 100))

small.show()
```

My Use-Case: For when my images need to be thumbnail-sized — like my ambitions after a failed merge conflict

#### Cropping 

```python
cropped = image.crop((100, 100, 400, 400))

cropped.show()
```

My Use-Case: Great for when eliminating that one friend - and we all have one - that blinks in every single photo we have ever taken since we were six, in my case. 

#### Rotating 

```python
rotated = image.rotate(90)

rotated.show()
```

My Use-Case: I don't really have one. But one that could be due since I am about to enter the realms of middle-age crisis, this boss of a script would be handy when I will want to see things from a different perspective - off the top of my head... 90 degrees of existential crisis? What do you think? 

#### Converting to B&W

```python
bw = image.convert("L")

bw.show()
```

My Use-Case: Perfect for turning joys into grayscale. In my case, it also worked for ‘serious coder’ profile pics. That is a true thing - check it my [LinkedIn profile](https://www.linkedin/in/nkleovoulou)

**Saving your hard work**

```python
bw.save("sad_your_picture_of_choice.png")
```

> No use case. Save your work. Have proof when family members questions your intelligence or put you down. Show them with pride and say: "I did that in programming. Your brownie points are up. You won.

And here, we are reaching the end of my very long guide. I hope you have enjoyed reading it. 

Pillow isn't just what I mentioned here or the way I describe it. It is a fun way, and sometimes the only way for me to advance my coding skills. And so if one other person enjoys taking their first steps like this, then this is what I am publishing them for. 

And for the Pillow grown ups, links to each of the actions described recklessly above are provide below:

1. [Image Resize](https://pillow.readthedocs.io/en/stable/reference/Image.html#PIL.Image.Image.resize) 
2. [Image Crop](https://pillow.readthedocs.io/en/stable/reference/Image.html#PIL.Image.Image.crop)
3. [Image Rotate](https://pillow.readthedocs.io/en/stable/reference/Image.html#PIL.Image.Image.rotate)
4. [Image Convert](https://pillow.readthedocs.io/en/stable/reference/Image.html#PIL.Image.Image.convert)
5. [Image Save](https://pillow.readthedocs.io/en/stable/reference/Image.html#PIL.Image.Image.save)

> \#Python, #Pillow, #ImageProcessing, #BeginnerFriendly, #PythonHumor, #ProgrammersWhoCry