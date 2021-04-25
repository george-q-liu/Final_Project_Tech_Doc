<!-- PROJECT LOGO -->
<br />
<p align="center">

  <h3 align="center">ENGCMP 1101 Final Project</h3>

  <p align="center">
    Instructor: Emelyn Catherine Smith-Ferris
  </p>
  <p align="center">
    An AI-Powered Chatbot to Ease Communication Issues!
  </p>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li><a href="#database">Database</a></li>
    <li><a href="#model-trainning">Database</a></li>
    <li>
      <a href="#getting-started">Getting Started</a>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

This final project will attempt to address the issue I mentioned in my communication issue presentation and extend on that topic. To address the issue caused by inadequate communication between Computer Science TAs and Professors, I have been working to develop this Artificial Intelligence-powered (AI) chatbot using my front-end development skills as a personal project. With this tool, professors can set up their own version of the chatbot and make necessary modifications. Students and UTAs can then use this chatbot to get instant responses from their professors for most of their inquiry. If a question submitted by student is not correctly received or answered by the chatbot, the student can provide feedback on the chatbot to alert their professor that a human response is needed. During this process, students should feel less intimidated by their professor and UTAs will have more opportunities to talk to their professor, thus alleviating the communication issue.  

Because the chatbot need to understand user input (questions in English, a natural language), an AI-powered natural language processing (NLP) engine is needed, and this engine is the most significant part of this project. Presentation of the chatbot on the website is trivial compared to the development of the AI NLP engine. The complete back-end AI NLP engine uses prepared intent inputs to generate several AI model files. The AI NLP engine has been integrated into the website so users can interact with the back-end AI NLP engine using the front-end chatbot application. 

### Built With

This web application is build on the foundation of the following major framworks. (see Acknowledgements section for more project dependencies)
* [Bootstrap](https://getbootstrap.com)
* [TensorFlow](https://www.tensorflow.org)
* [Flask](https://flask.palletsprojects.com/en/1.1.x/)
* [scikit-learn (sklearn)](https://scikit-learn.org/stable/)


<!-- Database -->
## Database

Amazon DynamoDB, a fully managed proprietary NoSQL database, was used as the database in this project.

1.Create your own [AWS account](https://aws.amazon.com/)

2.Create **Question_list** table with **Question ID (String)** as Primary partition key; **Category (String)** as Global Secondary Indexes. 

3.Create **Courses_Schedule** table with **Class Number (String)** as Primary partition key; **Course Number (String)** as Global Secondary Indexes. 

4.Create **Pitt_CS_Faculty** table with **Full Name (String)** as Primary partition key.

5.Create **Pitt_CS_Courses** table with **Course ID (String)** as Primary partition key.

6.Create **Add_Questions** table with **Questions (String)** as Primary partition key.

7.Run **DynamoDB.py** to upload local data to DynamoDB
  ```sh
  $ python3 DynamoDB.py
  ```


<!-- Model Trainning -->
## Model Trainning
By running the train_Vkathy.py, we will build and train the deep learning model that can classify and identify what the user is asking the bot.

- AI model files can be found in the TrainedModel files folder.
- The new model needs to be trained once any modification made to the intents file. 



<!-- GETTING STARTED -->
## Getting Started

This is a step-by-step guide on how to install Virtual Kathy on your machine and set up a python3 virtual environment.

### Prerequisites & Installation

Because Virtual Kathy is a web application build using Flask framework with Python 3, we need to set up a python 3 virtual environment and activate it.

1. Clone this git repo to your local machine

2. Download a python3 virtual environment (venv).
  ```sh
  $ python3 -m venv venv
  ```
3. Then activate python3 venv.
  ```sh
  $ . venv/bin/activate
  ```
4. Install all dependencies
 ```sh
  $ pip install -r requirements.txt
  ```
5. Export Virtual Kathy as a Flask Application
 ```sh
  $ export FLASK_APP=main.py
  ```
7. Run Virtual Kathy
 ```sh
  $ flask run
  ```



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

George Liu - georgeliu@pitt.edu



<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Img Shields](https://shields.io)
* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Pages](https://pages.github.com)
* [Animate.css](https://daneden.github.io/animate.css)
* [Loaders.css](https://connoratherton.com/loaders)
* [Slick Carousel](https://kenwheeler.github.io/slick)
* [Smooth Scroll](https://github.com/cferdinandi/smooth-scroll)
* [Sticky Kit](http://leafo.net/sticky-kit)
* [JVectorMap](http://jvectormap.com)
* [Font Awesome](https://fontawesome.com)





<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
