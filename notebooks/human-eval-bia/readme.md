
# List of use-cases
This list of use-cases is auto-generated. Do not modify this file.


* [detect_edges](human-eval-bia/filtering_0.ipynb): 
    Applies an edge-detection filter to an image.
    
        
* [remove_noise_edge_preserving](human-eval-bia/filtering_1.ipynb): 
    Applies an edge-preserving noise-removal filter to an image.
    
        
* [return_hello_world](human-eval-bia/hello_world.ipynb): 
    Returns the string "hello world".
    
        
* [remove_labels_on_edges](human-eval-bia/label_processing_0.ipynb): 
    Takes a label_image and removes all objects which touch the image border.
    
        
* [label_sequentially](human-eval-bia/label_processing_1.ipynb): 
    Takes a label_image with n labels and relabels the objects, 
    to make sure all integer labels between 0 and n are used. 
    No gaps are there.
    
        
* [remove_small_labels](human-eval-bia/label_processing_2.ipynb): 
    Takes a label_image and removes all objects that are smaller than a given size_threshold.
    
        
* [expand_labels_without_overlap](human-eval-bia/label_processing_3.ipynb): 
    Takes a label_image and enlarges all labels by a given radius, without
    labels overwriting each other.
    
        
* [binary_closing](human-eval-bia/label_processing_4.ipynb): 
    Applies binary closing to a binary_image with a square footprint with a given radius.
    
        
* [measure_intensity_of_labels](human-eval-bia/measure_0.ipynb): 
    Takes a label image and an intensity image, and returns a list of mean intensities 
    of all pixels in the intensity image, belonging to a given label.
    
        
* [measure_pixel_count_of_labels](human-eval-bia/measure_1.ipynb): 
    Takes a label image and returns a list of counts of number of pixels per label.
    
        
* [measure_mean_image_intensity](human-eval-bia/measure_2.ipynb): 
    Takes an image and returns its mean intensity
    
        
* [measure_properties_of_regions](human-eval-bia/measure_3.ipynb): 
    Takes a label image and an intensity image, and returns pandas dataframe
    with measurements for area, perimeter and mean_intensity.
    
        
* [count_overlapping_regions](human-eval-bia/measure_4.ipynb): 
    Takes two label images and counts how many objects in label_image_1 overlap 
    with any label in label_image_2 with at least one pixel.
    It returns the count of overlapping objects.
    
        
* [count_number_of_touching_neighbors](human-eval-bia/measure_5.ipynb): 
    Takes a label image and returns a list of number of touching neighbors 
    for each labeled object.
    
        
* [maximum_intensity_projection](human-eval-bia/project_0.ipynb): 
    Performs a maximum intensity projection along the first axis of an image.
    
        
* [sum_intensity_projection](human-eval-bia/project_1.ipynb): 
    Performs a maximum intensity projection along the first axis of an image.
    
        
* [label_binary_image_and_count_labels](human-eval-bia/segmentation_0.ipynb): 
    Consumes as input a binary image, applies connected component labeling to it, 
    counts the labeled objects and returns their count as single number.
    
        
* [apply_otsu_threshold_and_count_postiive_pixels](human-eval-bia/segmentation_1.ipynb): 
    Takes an image, applies Otsu's threshold method to it to create a binary image and 
    counts the positive pixels.
    
        
* [region_growing_segmentation](human-eval-bia/segmentation_2.ipynb): 
    Segments an image using the region-growing/flood filling 
    starting from a single point.
    
        
* [crop_quarter_image](human-eval-bia/transform_0.ipynb): 
    Crops out the first half image in both dimensions (width and height). 
    The resulting image will be of quarter size compared to the original image.
    
        
* [crop_quarter_image](human-eval-bia/transform_1.ipynb): 
    Crops out the first half image in both dimensions (width and height). 
    The resulting image will be of quarter size compared to the original image.
    
        
* [rotate_image_by_90_degrees](human-eval-bia/transform_2.ipynb): 
    Rotates an image by 90 degrees clockwise around the center of the image.
    
        
* [subsample_image](human-eval-bia/transform_3.ipynb): 
    Subsamples an image by taking the skipping every n'th pixel in X and Y.
    
        
* [worflow_segmentation_measurement_summary](human-eval-bia/workflow_0.ipynb): 
    This function implements a workflow consisting of these steps:
    * threshold intensity input image using Otsu's method
    * label connected components
    * measure area of the labeled objects
    * determine mean area of all objects
    
        
* [worflow_watershed_segmentation_correction_measurement](human-eval-bia/workflow_1.ipynb): 
    This function implements a workflow consisting of these steps:
    * blurs the image a bit
    * detect local minima in the blurred image
    * apply watershed segmentation flooding the blurred image from the 
      detected minima to retrieve a label image
    * remove all objects which touch the image border
    * measure the area of all remaining objects together
    
        
* [worflow_segmentation_counting](human-eval-bia/workflow_2.ipynb): 
    This function segments objects in an image with intensity above average 
    and returns their count.
    
        