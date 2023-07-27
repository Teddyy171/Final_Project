Sign Language Translator

This project uses a jetson nano and a USB camera to translate sign language. It will translate whatever sign you hold up into a aplhabet. 

## The Algorithm
Before I say anything, I have to say that I used the Nvidia template on Jupyter in order to make this project.
The first thing I had to do was get a dataset. Instead of getting one from online, I decided to make my own! So I used the USB Logitech camera to take images of myself doing the hand signs. Since I had 85-100 photos for each letter and theres 26 letters in the alphabet the math adds up to somewhere around 2,450 images to train off of. Once I got the dataset, I used Pytorch to start training with image classification. Image classification uses convolutional networks to dilute it down to certain images which will then be compared with others and use patterns to decide what the prediction will be. This process took 7+ hours to train since theres a lot of photos meanwhile I'm using the nano. The final project will take the image your presenting in front the camera and will give the answer back into the prediction box. 

## Running this project

1. Connect your USB webcam to your nano
2. Then turn on the nano
3. Enter the docker using the line ./docker_dli_run.sh, then enter your password.
4. Once you've done that, a https website link should show up with a password for that site. Go to that website and enter the password.
5. Next take the main file of this repo and download it.
6. Upload the code file into the jupyter webite.
7. To finish the setup you will need to click the run button which can be found above the tabs of code.
8. Keep on clicking until you meet the line of text that says, "Before you go Shut down the camera and/or notebook kernel to release the camera resource."
9. Scroll up to the new part with the camera output. There you should be ready to go once you click the "Live" button. 
10. Put up some sign language and watch as the prediction tells you what letter of the alphabet your holding up.

View the video demonstration here -----> (video link)
