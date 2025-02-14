# AI-driven physics game engine

Final project for the Building AI course

## Summary

This project explores the use of AI to approximate game physics, reducing the need for computationally expensive calculations. By training a model on precomputed physics simulations, the AI can predict outcomes with high accuracy, enabling smoother and more efficient real-time gameplay. Traditional physics engines rely on numerical solvers, which can be computationally expensive, especially for complex collisions, fluid dynamics, or soft-body simulations. AI can help by learning from past simulations and predicting results, reducing the need for constant recalculations.

## Background

It solves the need to perform sometimes really heavy computation either server side, or client side, in games when trying to simulate physical events. Most games with good destruction or physics will present it as a primary selling point, as it takes away from much else. Physics in games can also feel static, or scripted, materials will feel the same and there are obvious flaws in most interactions. 

## How is it used?

The AI model is trained on precomputed physics simulations (e.g., projectile motion, collisions, ragdoll physics). During gameplay, instead of running a full physics simulation, the AI quickly predicts the outcome of interactions. Game engines can integrate this model to optimize calculations in physics-heavy scenarios (e.g., destructible environments, fluid physics, soft bodies). Given more AI oriented GPU structures of recent cards, this should be more accessible to approach as well.

Images will make your README look nice!
Once you upload an image to your repository, you can link link to it like this (replace the URL with file path, if you've uploaded an image to Github.)
![Cat](https://upload.wikimedia.org/wikipedia/commons/5/5e/Sleeping_cat_on_her_back.jpg)

If you need to resize images, you have to use an HTML tag, like this:
<img src="https://upload.wikimedia.org/wikipedia/commons/5/5e/Sleeping_cat_on_her_back.jpg" width="300">

This is how you create code examples:
```
def main():
   countries = ['Denmark', 'Finland', 'Iceland', 'Norway', 'Sweden']
   pop = [5615000, 5439000, 324000, 5080000, 9609000]   # not actually needed in this exercise...
   fishers = [1891, 2652, 3800, 11611, 1757]

   totPop = sum(pop)
   totFish = sum(fishers)

   # write your solution here

   for i in range(len(countries)):
      print("%s %.2f%%" % (countries[i], 100.0))    # current just prints 100%

main()
```


## Data sources and AI methods
## Challenges

It doesnt entirely eliminate the need for computational power, but rather frontloads it into the simulations you run to teach your AI or ml algo to predict better. Which for rather large studios should be fine, but for smaller, less accessible, and it might widen the gap. Altough I'm sure some engine like unreal would incorporate it into their engine at some point.

## What next?

I think this would be possible to essentially proof of concept on my own, with some time. But to showcase real feasibility it would almost need to be trained on larger amounts of data. I am an undergrad in physics, but my current gamedev knowledge is limited to physics simulation, and as such would most likely need a team of AI and game developers.


## Acknowledgments

* list here the sources of inspiration 
* do not use code, images, data etc. from others without permission
* when you have permission to use other people's materials, always mention the original creator and the open source / Creative Commons licence they've used
  <br>For example: [Sleeping Cat on Her Back by Umberto Salvagnin](https://commons.wikimedia.org/wiki/File:Sleeping_cat_on_her_back.jpg#filelinks) / [CC BY 2.0](https://creativecommons.org/licenses/by/2.0)
