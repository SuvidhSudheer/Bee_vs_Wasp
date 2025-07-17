# Bee_vs_Wasp

Bee_vs_Wasp is a simple AI recognition project that is used to differentiate between bees and wasps in pictures. This project does only currently differentiate between wasps and bees with hornets and other similar insects being labeled under bee or wasp depending on which one it looks the most like.

![test](https://github.com/user-attachments/assets/d0156474-0088-413f-a743-a38effebdda2)

## The Algorithm

This project uses jetson-inference and resnet to analyze photos provided for traits present in both wasps and bees, able to distinguish the two from eachother and detect them in images.

## Running this project

1. Clone the Bee_vs_Wasp Project by downloading it from GitHub:
2. Extract the folder
3. Open in VS Code
4. Make sure you have the python add-ons installed
5. Open a terminal (Terminal > New Terminal)
6. Navigate into your main folder
15. Set the NET and DATASET variables:
  NET=models/bee_wasp
  DATASET=data/bee_wasp
16. Run this command to see how it operates on an image from the test folder.
      imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --    labels=$DATASET/labels.txt $DATASET/test/bee or wasp/name of test file.jpg outputname.jpg
17. Run the same command with whichever file you would want to test.

This is a video demonstration of the project
https://github.com/user-attachments/assets/b7e3e310-e83e-4f58-b25f-bdfc0ea667a1


