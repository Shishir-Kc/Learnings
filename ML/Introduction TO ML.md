
Machine learning (ML) powers some of the most important technologies we use, from translation apps to autonomous vehicles. This course explains the core concepts behind ML.

ML offers a new way to solve problems, answer complex questions, and create new content. ML can predict the weather, estimate travel times, recommend songs, auto-complete sentences, summarize articles, and generate never-seen-before images.

In basic terms, ML is the process of [training](https://developers.google.com/machine-learning/glossary#training) a piece of software, called a [model](https://developers.google.com/machine-learning/glossary#model), to make useful [predictions](https://developers.google.com/machine-learning/glossary#prediction) or generate content (like text, images, audio, or video) from data.

For example, suppose we wanted to create an app to predict rainfall. We could use either a traditional approach or an ML approach. Using a traditional approach, we'd create a physics-based representation of the Earth's atmosphere and surface, computing massive amounts of fluid dynamics equations. This is incredibly difficult.

Using an ML approach, we would give an ML model enormous amounts of weather data until the ML model eventually _learned_ the mathematical relationship between weather patterns that produce differing amounts of rain. We would then give the model the current weather data, and it would predict the amount of rain.

## Types of ML Systems

ML systems fall into one or more of the following categories based on how they learn to make predictions or generate content:

- Supervised learning
- Unsupervised learning
- Reinforcement learning
- Generative AI

## Supervised learning

[Supervised learning](https://developers.google.com/machine-learning/glossary#supervised-machine-learning) models can make predictions after seeing lots of data with the correct answers and then discovering the connections between the elements in the data that produce the correct answers. This is like a student learning new material by studying old exams that contain both questions and answers. Once the student has trained on enough old exams, the student is well prepared to take a new exam. These ML systems are "supervised" in the sense that a human gives the ML system data with the known correct results.

Two of the most common use cases for supervised learning are regression and classification.

### Regression

A [regression model](https://developers.google.com/machine-learning/glossary#regression-model) predicts a numeric value. For example, a weather model that predicts the amount of rain, in inches or millimeters, is a regression model.

See the table below for more examples of regression models:

| Scenario           | Possible input data                                                                                                                                                            | Numeric prediction                                          |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------- |
| Future house price | Square footage, zip code, number of bedrooms and bathrooms, lot size, mortgage interest rate, property tax rate, construction costs, and number of homes for sale in the area. | The price of the home.                                      |
| Future ride time   | Historical traffic conditions (gathered from smartphones, traffic sensors, ride-hailing and other navigation applications), distance from destination, and weather conditions. | The time in minutes and seconds to arrive at a destination. |

### Classification

[Classification models](https://developers.google.com/machine-learning/glossary#classification-model) predict the likelihood that something belongs to a category. Unlike regression models, whose output is a number, classification models output a value that states whether or not something belongs to a particular category. For example, classification models are used to predict if an email is spam or if a photo contains a cat.

Classification models are divided into two groups: binary classification and multiclass classification. Binary classification models output a value from a class that contains only two values, for example, a model that outputs either `rain` or `no rain`. Multiclass classification models output a value from a class that contains more than two values, for example, a model that can output either `rain`, `hail`, `snow`, or `sleet`.

## Unsupervised learning

An [unsupervised learning](https://developers.google.com/machine-learning/glossary#unsupervised-machine-learning) model aims to identify meaningful patterns in a dataset. For example, many unsupervised learning models rely on a technique called [clustering](https://developers.google.com/machine-learning/glossary#clustering) to organize similar data into groups ("clusters").

![An image showing colored dots in clusters.](https://developers.google.com/static/machine-learning/intro-to-ml/images/clustering-02.png)

**Figure 1**. An ML model clustering similar data points.

![An image showing colored dots in clusters that are enclosed in a shape and border each other.](https://developers.google.com/static/machine-learning/intro-to-ml/images/clustering-04.png)

**Figure 2**. Groups of clusters with natural demarcations.

Clustering differs from classification because the categories aren't defined by you. For example, an unsupervised model might cluster a weather dataset based on temperature, revealing segmentations that define the seasons. You might then attempt to name those clusters based on your understanding of the dataset.

![An image showing colored dots in clusters that are labeled as snow, rain, hail, and no rain.](https://developers.google.com/static/machine-learning/intro-to-ml/images/clustering-01.png)

**Figure 3**. An ML model clustering similar weather patterns.

![An image showing colored dots in clusters that are labeled as snow, rain, hail, and no rain that are enclosed in a shape and border each other.](https://developers.google.com/static/machine-learning/intro-to-ml/images/clustering-03.png)

**Figure 4**. Clusters of weather patterns labeled as snow, sleet, rain, and no rain.

## Reinforcement learning

[Reinforcement learning](https://developers.google.com/machine-learning/glossary#reinforcement-learning-rl) models make predictions by getting [rewards](https://developers.google.com/machine-learning/glossary#reward) or penalties based on actions performed within an environment. A reinforcement learning system generates a [policy](https://developers.google.com/machine-learning/glossary#policy) that defines the best strategy for getting the most rewards.

Reinforcement learning is used to train robots to perform tasks, like walking around a room, and software programs like [AlphaGo](https://deepmind.com/research/case-studies/alphago-the-story-so-far) to play the game of Go.


## Generative AI

[Generative AI](https://developers.google.com/machine-learning/glossary#generative-ai) is a class of models that creates content from user input. For example, generative AI can create unique images, music compositions, and jokes; it can summarize articles, explain how to perform a task, or edit a photo.

Generative AI can take a variety of inputs and create a variety of outputs, like text, images, audio, and video. It can also take and create combinations of these. For example, a model can take an image as input and create an image and text as output, or take an image and text as input and create a video as output.

We can discuss generative models by their inputs and outputs, typically written as "type of input"-to-"type of output." For example, the following is a partial list of some inputs and outputs for generative models:

- Text-to-text
- Text-to-image
- Text-to-video
- Text-to-code
- Text-to-speech
- Image and text-to-image

The following table contains examples of generative models, their input, and their possible output:

|Model|Input|Example output|
|---|---|---|
|Text-to-text|Who invented the Le Mans race?|The 24 Hours of Le Mans was founded by the Automobile Club de l'Ouest (ACO), a motoring organization founded in 1906. The first race was held on 26 and 27 May 1923 on the Sarthe Circuit, a 13.426-kilometre (8.345-mile) road circuit located near the town of Le Mans in France. The race was originally conceived as a way to promote the ACO and the Sarthe region.  <br>Source: [Bard](https://bard.google.com)|
|Text-to-image|An alien octopus floats through a portal while reading a newspaper.|![Image of a cartoon octopus.](https://developers.google.com/static/machine-learning/intro-to-ml/images/octopus.png)  <br>Source: [Imagen](https://imagen.research.google/)|
|Text-to-video|A photorealistic teddy bear is swimming in the ocean at San Francisco. The teddy bear goes under water. The teddy bear keeps swimming under the water with colorful fishes. A panda bear is swimming under water.|![Video of a teddy bear swimming underwater.](https://developers.google.com/static/machine-learning/intro-to-ml/images/teddy_bear.gif)  <br>Source: [Phenaki](https://phenaki.video/)|
|Text-to-code|Write a Python loop that loops over a list of numbers and prints the prime numbers.|for number in numbers:<br>  # Check if the number is prime.<br>  is_prime = True<br>  for i in range(2, number):<br>    if number % i == 0:<br>        is_prime = False<br>        break<br>  # If the number is prime, print it.<br>  if is_prime:<br>    print(number)<br><br>  <br>Source: [Bard](https://bard.google.com)|
|Image-to-text|![Image of a flamingo.](https://developers.google.com/static/machine-learning/intro-to-ml/images/flamingo.png)|This is a flamingo. They are found in the Caribbean.  <br>Source: [Google DeepMind](https://www.deepmind.com/blog/tackling-multiple-tasks-with-a-single-visual-language-model)|

How does generative AI work? At a high-level, generative models learn patterns in data with the goal to produce new but similar data. Generative models are like the following:

- Comedians who learn to imitate others by observing people's behaviors and style of speaking
- Artists who learn to paint in a particular style by studying lots of paintings in that style
- Cover bands that learn to sound like a specific music group by listening to lots of music by that group

To produce unique and creative outputs, generative models are initially trained using an unsupervised approach, where the model learns to mimic the data it's trained on. The model is sometimes trained further using supervised or reinforcement learning on specific data related to tasks the model might be asked to perform, for example, summarize an article or edit a photo.

Generative AI is a quickly evolving technology with new use cases constantly being discovered. For example, generative models are helping businesses refine their ecommerce product images by automatically removing distracting backgrounds or improving the quality of low-resolution images.


**Key Terms:**

- [classification model](https://developers.google.com/machine-learning/glossary#classification-model)
- [clustering](https://developers.google.com/machine-learning/glossary#clustering)
- [model](https://developers.google.com/machine-learning/glossary#model)
- [policy](https://developers.google.com/machine-learning/glossary#policy)
- [prediction](https://developers.google.com/machine-learning/glossary#prediction)
- [regression model](https://developers.google.com/machine-learning/glossary#regression-model)
- [reinforcement learning](https://developers.google.com/machine-learning/glossary#reinforcement-learning-rl)
- [reward](https://developers.google.com/machine-learning/glossary#reward)
- [supervised learning](https://developers.google.com/machine-learning/glossary#supervised-machine-learning)
- [training](https://developers.google.com/machine-learning/glossary#training)
- [unsupervised learning](https://developers.google.com/machine-learning/glossary#unsupervised-machine-learning)