
# List of use-cases
This list of 57 use-cases is auto-generated. Do not modify this file.


* [apply_otsu_threshold_and_count_postiive_pixels](apply_otsu_threshold_and_count_postiive_pixels.ipynb): 
    Takes an image, applies Otsu's threshold method to it to create a binary image and 
    counts the positive pixels.
    
        
* [binary_closing](binary_closing.ipynb): 
    Applies binary closing to a binary_image with a square footprint with a given radius.
    
        
* [binary_skeleton](binary_skeleton.ipynb): 
    Applies skeletonization to a 2D binary image.
    
        
* [bland_altman](bland_altman.ipynb): 
    Takes two specified columns from a given dataframe and applies Bland-Altman-Analysis to them.
    Therefore, it adds two new columns, one called 'mean' containing the mean of the two corresponding values,
    and one called 'diff' containing the difference between the two.
    
        
* [combine_columns_of_tables](combine_columns_of_tables.ipynb): 
    This function combines to dataframes and makes sure the data is merged 
    using the given index column, which must be present in both dataframes.
    The dataframes should be merged in a way that no data is lost and missing
    fields are filled with NaN.
    
        
* [convex_hull_measure_area](convex_hull_measure_area.ipynb): 
    Take a 3D point_cloud, determines the convex hull around the points and returns the surface area of the convex hull.
    
        
* [convolve_images](convolve_images.ipynb): 
    Convolve an image with a kernel_image and return the result
    
        
* [count_number_of_touching_neighbors](count_number_of_touching_neighbors.ipynb): 
    Takes a label image and returns a list of number of touching neighbors 
    for each labeled object.
    
        
* [count_objects_over_time](count_objects_over_time.ipynb): 
    Takes a timelapse (list of binary images), counts the number of connected components and returns the resulting counts as list.
    
        
* [count_overlapping_regions](count_overlapping_regions.ipynb): 
    Takes two label images and counts how many objects in label_image_1 overlap 
    with any label in label_image_2 with at least one pixel.
    It returns the count of overlapping objects.
    
        
* [create_umap](create_umap.ipynb): 
    Takes a dataframe and computes a UMAP from all columns. 
    The two UMAP vectors are stored in the dataframe as `umap0` and `umap1`.
    
        
* [crop_quarter_image](crop_quarter_image.ipynb): 
    Crops out the first half image in both dimensions (width and height). 
    The resulting image will be of quarter size compared to the original image.
    
        
* [deconvolve_image](deconvolve_image.ipynb): 
    Deconvolve an image with a kernel_image and return the result.
    
        
* [detect_edges](detect_edges.ipynb): 
    Applies an edge-detection filter to an image.
    
        
* [expand_labels_without_overlap](expand_labels_without_overlap.ipynb): 
    Takes a label_image and enlarges all labels by a given radius, without
    labels overwriting each other.
    
        
* [extract_surface_measure_area](extract_surface_measure_area.ipynb): 
    Take a 3D binary_volume_image, extracts the surface of the white (voxel value != 0) object 
    and returns the surface area of the object.
    
        
* [fit_circle](fit_circle.ipynb): 
    Implements 2D circle fitting
    Input: Collection of 2d points, represented as a list of lists [ [x0,y0], [x1,y1], ... ]  
    Output: Tuple: xc, yc, radius
    
        
* [label_binary_image_and_count_labels](label_binary_image_and_count_labels.ipynb): 
    Consumes as input a binary image, applies connected component labeling to it, 
    counts the labeled objects and returns their count as single number.
    
        
* [label_sequentially](label_sequentially.ipynb): 
    Takes a label_image with n labels and relabels the objects, 
    to make sure all integer labels between 0 and n are used. 
    No gaps are there.
    
        
* [list_image_files_in_folder](list_image_files_in_folder.ipynb): 
    Lists all image files in a folder.
    
        
* [map_pixel_count_of_labels](map_pixel_count_of_labels.ipynb): 
    Takes a label_image, determines the pixel-count per label and creates an image where the label values are replaced by the corresponding pixel count.
    
        
* [mask_image](mask_image.ipynb): 
    Takes a 2D input image and a 2D binary mask image, then applies the mask to the input image and returns the result.
    
        
* [maximum_intensity_projection](maximum_intensity_projection.ipynb): 
    Performs a maximum intensity projection along the first axis of an image.
    
        
* [mean_squared_error](mean_squared_error.ipynb): 
    Computes the mean-squared-error of two images compared pixel-by-pixel
    
        
* [mean_std_column](mean_std_column.ipynb): 
    Computes the mean average and standard deviation of a specified column 
    in a given dataframe and returns these two values.
    
        
* [measure_aspect_ratio_of_regions](measure_aspect_ratio_of_regions.ipynb): 
    Takes a label image and returns a pandas dataframe
    with measurements for aspect_ratio of the objects
    
        
* [measure_intensity_of_labels](measure_intensity_of_labels.ipynb): 
    Takes a label image and an intensity image, and returns a list of mean intensities 
    of all pixels in the intensity image, belonging to a given label.
    
        
* [measure_intensity_over_time](measure_intensity_over_time.ipynb): 
    Takes a timelapse (list of images), measures the average intensity over time and returns the resulting measurements as list.
    
        
* [measure_mean_image_intensity](measure_mean_image_intensity.ipynb): 
    Takes an image and returns its mean intensity
    
        
* [measure_pixel_count_of_labels](measure_pixel_count_of_labels.ipynb): 
    Takes a label image and returns a list of counts of number of pixels per label.
    
        
* [measure_properties_of_regions](measure_properties_of_regions.ipynb): 
    Takes a label image and an intensity image, and returns pandas dataframe
    with measurements for area, perimeter and mean_intensity.
    
        
* [open_image_read_voxel_size](open_image_read_voxel_size.ipynb): 
    Reads an image file and return its voxel size in Z-Y-X order.
    
        
* [open_image_return_dimensions](open_image_return_dimensions.ipynb): 
    Opens an image and returns its dimensions
    
        
* [open_nifti_image](open_nifti_image.ipynb): 
    This function loads a nifti image from the file at image_location and returns the image data as a numpy array. 
    
        
* [open_zarr](open_zarr.ipynb): 
    Opens a zarr file and returns the array
    
        
* [pair_wise_correlation_matrix](pair_wise_correlation_matrix.ipynb): 
    Takes a pandas dataframe and computes for all columns their Pearson's correlation coefficient
    for all columns in the dataframe. For n columns, this is a n x n matrix of coefficients.
    The matrix is returned as dataframe.
    
        
* [radial_intensity_profile](radial_intensity_profile.ipynb): 
    Computes the radial intensity profile of an image around a given coordinate
    Inputs:
    - image: 2d numpy array
    - xy, yc: the center coordinates
    Output:
    - an array containing the average intensities
    
        
* [region_growing_segmentation](region_growing_segmentation.ipynb): 
    Segments an image using the region-growing/flood filling 
    starting from a single point.
    
        
* [remove_labels_on_edges](remove_labels_on_edges.ipynb): 
    Takes a label_image and removes all objects which touch the image border.
    
        
* [remove_noise_edge_preserving](remove_noise_edge_preserving.ipynb): 
    Applies an edge-preserving noise-removal filter to an image.
    
        
* [remove_small_labels](remove_small_labels.ipynb): 
    Takes a label_image and removes all objects that are smaller than a given size_threshold.
    
        
* [return_hello_world](return_hello_world.ipynb): 
    Returns the string "hello world".
    
        
* [rgb_to_grey_image_transform](rgb_to_grey_image_transform.ipynb): 
    Convert an RGB image to a single-channel gray scale image with 
    configurable weights r, g and b.
    The weights are normalized to be 1 in sum.
    
        
* [rotate_image_by_90_degrees](rotate_image_by_90_degrees.ipynb): 
    Rotates an image by 90 degrees clockwise around the center of the image.
    
        
* [subsample_image](subsample_image.ipynb): 
    Subsamples an image by skipping every n'th pixel in X and Y.
    
        
* [subtract_background_tophat](subtract_background_tophat.ipynb): 
    Applies a top-hat filter with a given radius to an image with dark background (low values) and bright foreground (high values).
    
        
* [sum_images](sum_images.ipynb): 
    Sums two images pixel-by-pixel and returns the result
    
        
* [sum_intensity_projection](sum_intensity_projection.ipynb): 
    Performs a maximum intensity projection along the first axis of an image.
    
        
* [tiled_image_processing](tiled_image_processing.ipynb): 
    Apply a maximum filter with a given radius to the image using a tile-by-tile strategy.
    The tile_size denotes the size of the tiles in X and Y.
    
        
* [transpose_image_axes](transpose_image_axes.ipynb): 
    Transposes the first two axes of an image.
    
        
* [t_test](t_test.ipynb): 
    Takes two specified columns from a given dataframe and applies a paired T-test to it to determine the p-value.
    
        
* [workflow_batch_process_folder_count_labels](workflow_batch_process_folder_count_labels.ipynb): 
    This functions goes through all .tif image files in a specified folder, 
    loads the images and count labels each image. 
    It returns a dictionary with filenames and corresponding counts.
    
        
* [workflow_batch_process_folder_measure_intensity](workflow_batch_process_folder_measure_intensity.ipynb): 
    This functions goes through all .tif image files in a specified image folder 
    and corresponding label images in another labels folder. 
    It loads the images and corresponding labels, and measures min, mean and max intensity of all labels.
    The function returns a dataframe with five columns: min_intensity, mean_intensity, max_intensity, label and filename.
    
        
* [workflow_segmentation_counting](workflow_segmentation_counting.ipynb): 
    This function segments objects in an image with intensity above average 
    and returns their count.
    
        
* [workflow_segmentation_measurement_summary](workflow_segmentation_measurement_summary.ipynb): 
    This function implements a workflow consisting of these steps:
    * threshold intensity input image using Otsu's method
    * label connected components
    * measure area of the labeled objects
    * determine mean area of all objects
    
        
* [workflow_segment_measure_umap](workflow_segment_measure_umap.ipynb): 
    This function takes a single channel intensity image, 
    segments objects with intensity above half the maximum intensity, 
    labels connected components, 
    measures area, perimeter, mean_intensity, minor and major axis of the labeled objects, 
    and produces a UMAP from the given measurements. 
    The two UMAP vectors are saved as `umap0` and `umap1` togther with the measurements in a dataframe. 
    The function returns this dataframe.
    
        
* [workflow_watershed_segmentation_correction_measurement](workflow_watershed_segmentation_correction_measurement.ipynb): 
    This function implements a workflow consisting of these steps:
    * blurs the image a bit
    * detect local minima in the blurred image
    * apply watershed segmentation flooding the blurred image from the 
      detected minima to retrieve a label image
    * remove all objects which touch the image border
    * measure the area of all remaining objects together
    
        