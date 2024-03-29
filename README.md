# smart-playlist-generator
This program allows a user to enter a song and generates a playlist of similar songs using machine learning.

## User Guide
### Application Files
The application runs through a Jupyter Notebook utilizing ipywidgets to display user interface elements and Voila to run the code in its own window. In order to get the application up and running, make sure to closely follow the installation steps found within the user guide.
### Installation
This application utilizes Conda to streamline the installation process of all the necessary libraries.
If you don’t have Conda installed, go to https://docs.conda.io/projects/miniconda/en/latest/ and follow the instructions to install the appropriate version of Miniconda for your operating system.

<b>The following process will help you get up and running in just a of couple minutes:</b>
1. First save the folder titled “main_application” to your machine. Be sure to take note of the
folder’s filepath.
2. Open “Anaconda Prompt (Minconda3)”
3. Enter the command cd followed by the filepath of the main_application folder.  ie:

    ```cd C:\Users\user\Desktop\main_application\```
4. Enter the following command to create the environment and install the necessary libraries:

    ```conda create --prefix ./env pandas numpy matplotlib scikit-learn jupyter ipywidgets```
6. The following prompt will show:

    ```Proceed([y][n]?)```
7. Type ”y” and press enter.
   
8. Once the environment is successfully installed, use the following command to activate the
environment:

    ```conda activate ‘main_application-filepath’\env\```  
<sub>(Replace ‘main_application-filepath’ with the filepath of main_application ie: “conda activate C:
\Users\user\Desktop\main_application\env\”)</sub>

9. To install Voila enter the command:

    ```conda install -c conda-forge voila```  
10. Once again, enter ‘y’ to confirm.
12. Now that we have our libraries installed, we can enter the following command to launch the
application:

    ```voila app.ipynb```
14. The application will now open in a separate browser window

    <img width="372" alt="img1" src="https://github.com/Teeko98/smart-playlist-generator/assets/24867742/cdda7188-9470-4168-9094-89a678f4b798">

### Generating a playlist
1. Type out an artist, song, or an artist followed by song into the text field and click the search
button.  
<sub>(Note: If searching for a specific song by an artist, type out the full artist name followed by the song)</sub>.

    <img width="392" alt="img2" src="https://github.com/Teeko98/smart-playlist-generator/assets/24867742/63e8be26-d28f-4745-9ff5-b6881b3f435b">.

3. A selection box with matching results will be displayed.

    <img width="555" alt="img3" src="https://github.com/Teeko98/smart-playlist-generator/assets/24867742/10c1a22e-ea2d-401d-972c-6c10b8710d11">

5. Select the song you would like to generate the recommended playlist for and click the
‘Generate’ button.

    <img width="583" alt="img4" src="https://github.com/Teeko98/smart-playlist-generator/assets/24867742/1fb98de2-3ee3-4c12-a82b-0d40360c704c">.
   
7. The application will output a playlist of 30 songs in the form of a DataFrame with the artist
name, track name, and similarity score of each song.

    <img width="645" alt="img5" src="https://github.com/Teeko98/smart-playlist-generator/assets/24867742/a67eba61-af6b-4481-a441-29b246579561">
