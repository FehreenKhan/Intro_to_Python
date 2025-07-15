# Mars Weight

A few years ago, NASA made history with the first controlled flight on another planet. 
Its latest Mars Rover, Perseverance, has onboard a 50cm high helicopter called Ingenuity. 
Ingenuity made its third flight, during which it flew faster and further than it had on any of its test flights on Earth. 
Interestingly, Ingenuity uses Python  for some of its flight modeling software!

<img width="1200" height="675" alt="image" src="https://github.com/user-attachments/assets/46354c6a-4f5d-47cf-94db-692e7aec4934" />
(Source: NASA Science) 

When programming Ingenuity, one of the things that NASA engineers need to account for is the fact that due to the weaker gravity on Mars, an Earthling's weight on Mars is 37.8% of their weight on Earth.
Write a Python program that prompts an Earthling to enter their weight on Earth and prints their calculated weight on Mars. The output should be rounded to two decimal places when necessary.
Python has a round function which can help you with this. You pass in the value to be rounded and the number of decimal places to use.

# Figures to enter for a sample run: 

$ python marsweight.py

Enter a weight on Earth: 120

The equivalent weight on Mars: 45.36

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
"""
Prompts the user for a weight on Earth
and prints the equivalent weight on Mars.
"""

    
    def main(): 
        earth_weight = float(input("Enter a weight on Earth: "))
        #mars_weight = round(earth_weight *0.378, 2 )                                #the first few lines 34 to 37 will provide the weight on mars. 
        #print(f" The equivalent weight on Mars: {mars_weight}")
        # mars weight 

    #task 2 planetary weights calculator 
    planet = input("Enter a planet: ")                                       # task 2 shows the weight on another planet 
    #planets percentag figures, milestone 2 
    gravity_multipliers = {
        "Mercury": 0.376,
        "Venus": 0.889,
        "Mars": 0.378,
        "Jupiter": 2.36,
        "Saturn": 1.081,
        "Uranus": 0.815,
        "Neptune": 1.14
    }

    # multiplier from dictionary of planet names 
    multiplier = gravity_multipliers[planet]
    #equivalent weight on planet 
    planetary_weight = round(earth_weight * multiplier, 2)

    #to show the result
    print(f"The equivalent weight on {planet}:{planetary_weight}")

       if __name__ == "__main__":
          main()








Indentations are key and the code above is not properly indented due to extra notes with # within code to produce the calculations. 



# Haiku Generator 


Write a program to create a Haiku, using ai.
A haiku is a type of very short poem that originated in Japan. It has three lines. The first line has 5 syllables, the second has 7 syllables, and the third has 5 syllables again. Haiku usually describe a moment in nature or a feeling, using clear, simple images. Even though it is brief, a good haiku often gives the reader a quiet, thoughtful feeling.
Prompt the user to enter their name, and a topic. Then make use call_gpt to turn the name and topic into a haiku. We leave it up to you to come up with the prompt! Here are some sample runs:

For example: 

Enter your name: Freya
Enter a topic: Rain in the forest
Creating your haiku...

Freya roams the woods,  
Whispers dance with gentle rain,  
Nature's song remains.



Enter your name: Chris
Enter a topic: a global python classroom
Creating your haiku...

In the global space,  
Chris guides minds through Python's flow,  
Code unites us all.


Code to create Haiku Generator by importing the AI library via python. 

        from ai import call_gpt

         def main():
              name = input("Enter your name: ")
              topic = input("Enter a topic: ")
              prompt = f"write a haiku about {topic} addressed to {name}."
              print("Creating your haiku...")
              response = call_gpt(prompt)
              print(response)

         if __name__ == "__main__":
              main()


Notice the indentation for the code 






    







      
    













