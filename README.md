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

<img width="570" height="773" alt="image" src="https://github.com/user-attachments/assets/651c12ef-444f-436f-bf1e-5352683f904a" />

 









Indentations are key when writing code. 




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






    







      
    













