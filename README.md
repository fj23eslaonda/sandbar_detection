# Sand Bar Detection

This repository allows to identify sand bar using wave breaking patterns. To obtain wave breaking patterns is used a method propuse in [Wave-by-wave Nearshore Wave Breaking Identificationusing U-Net](https://github.com/fj23eslaonda/Wave_by_Wave_Identification) by Sáez et al. (2021). Main idea is to identify waves breaking frame by frame on a beach of interest and calculate the cumulative sum over all mask or patterns to create a cumulative breaking pixels map. Finally, algorithm detects all the maximum points on cumulative map to estimate the position of sand bar position.

## Inputs and parameters
| Parameter         | Description                           |
|-------------------|---------------------------------------|
| main_path         |  Main folder                          |
|image_path         | Image input folder                    |
|output_path        | Image output folder                   |
| beach_path        | Beach folder to save results          |
|plot_mask          | Boolean variable to save plots or not |
|plot_mask_over_img | Boolean variable to save plots or not |
| orientation       | Waves direction                       |

It's necessary to have rectified images of your beach of interest and it's very important than wave direction is from top to bottom of images ( or from right to left of images

