
# List of use-cases
This list of 57 use-cases is auto-generated. Do not modify this file.


* [apply_otsu_threshold_and_count_postiive_pixels](apply_otsu_threshold_and_count_postiive_pixels.ipynb): 
    Takes an image as numpy array, applies Otsu's threshold method to it to create a binary image and 
    counts the positive pixels and returns this number.
    
        
* [binary_closing](binary_closing.ipynb): 
    Applies binary closing with a square footprint with a given radius to a binary_image provided as numpy array and returns the result as numpy array.
    
        
* [binary_skeleton](binary_skeleton.ipynb): 
    Applies skeletonization to a 2D binary image provided as numpy array and returns the resulting skeleton image as numpy array.
    
        
* [bland_altman](bland_altman.ipynb): 
    Takes two columns specified by name from a given dataframe and applies Bland-Altman-Analysis to them.
    Therefore, it adds two new columns to the dataframe, one called 'mean' containing the mean of the two 
    corresponding values, and one called 'diff' containing the difference between the two.
    
        
* [combine_columns_of_tables](combine_columns_of_tables.ipynb): 
    This function combines to dataframes and makes sure the data is merged 
    using the given index column, which must be present in both dataframes.
    The dataframes should be merged in a way that no data is lost and missing
    fields are filled with NaN. The combined dataframe is returned.
    
        
* [convex_hull_measure_area](convex_hull_measure_area.ipynb): 
    Takes a 3D point_cloud as list of (Z,Y,X) coordinates, determines the convex hull around the points and returns the surface area of the convex hull.
    
        
* [convolve_images](convolve_images.ipynb): 
    Convolve an image with a kernel_image and return the result. All images are of type numpy array.
    
        
* [count_number_of_touching_neighbors](count_number_of_touching_neighbors.ipynb): 
    Takes a label image provided as numpy array and returns a list of number of touching neighbors 
    for each labeled object.
    
        
* [count_objects_over_time](count_objects_over_time.ipynb): 
    Takes a timelapse (list of binary images provided as numpy arrays), counts the number 
    of connected components for each time frame and returns the resulting counts as list.
    
        
* [count_overlapping_regions](count_overlapping_regions.ipynb): 
    Takes two label images provided as numpy arrays and counts how many objects in 
    label_image_1 overlap with any labeled object in label_image_2 with at least 
    one pixel. It returns the count of overlapping objects.
    
        
* [create_umap](create_umap.ipynb): 
    Takes a dataframe and computes a UMAP with 2 components from all columns. 
    The two UMAP vectors are stored in the dataframe as `umap0` and `umap1`.
    
        
* [crop_quarter_image](crop_quarter_image.ipynb): 
    Takes an image proved as numpy array, crops out the first half image in both dimensions (width and height). 
    The returned image will be of quarter size compared to the original image and of type numpy array.
    
        
* [deconvolve_image](deconvolve_image.ipynb): 
    Deconvolve an image with a kernel_image and return the result.
    Input images and return value are of type numpy array.
    
        
* [detect_edges](detect_edges.ipynb): 
    Applies an edge-detection filter to an image provided as numpy array and returns the result as numpy array.
    
        
* [expand_labels_without_overlap](expand_labels_without_overlap.ipynb): 
    Takes a label_image provided as numpy array and enlarges all labels by a given radius, without
    labels overwriting each other. The resulting label image is returned as numpy array.
    
        
* [extract_surface_measure_area](extract_surface_measure_area.ipynb): 
    Take a 3D binary_volume_image provided as numpy array, extracts the surface of the white (voxel value != 0) object 
    and returns the surface area of the object.
    
        
* [fit_circle](fit_circle.ipynb): 
    Fits a circle to points provided as list of (y,x) coordinates and 
    returns a tuple of (yc, xc, radius) describing the circle.
    
        
* [label_binary_image_and_count_labels](label_binary_image_and_count_labels.ipynb): 
    Takes a binary image provided as numpy array, applies connected component labeling to it, 
    counts the labeled objects and returns the count as single number.
    
        
* [label_sequentially](label_sequentially.ipynb): 
    Takes a label_image provided as numpy array with n labels and relabels the objects, 
    to make sure all integer labels between 0 and n are used and no gaps are there. 
    The resulting label image is returned as numpy array.
    
        
* [list_image_files_in_folder](list_image_files_in_folder.ipynb): 
    Given a folder_location as string, returns a list of all *.tif, *.jpg or *.png image files in a folder.
    
        
* [map_pixel_count_of_labels](map_pixel_count_of_labels.ipynb): 
    Takes a label_image provided as numpy array, determines the pixel-count per label and returns 
    a numpy-array image where the label values are replaced by the corresponding pixel count.
    
        
* [mask_image](mask_image.ipynb): 
    Takes a 2D input image and a 2D binary mask image, both provided as numpy array, 
    applies the mask to the input image and returns the result as numpy array.
    
        
* [maximum_intensity_projection](maximum_intensity_projection.ipynb): 
    Performs a maximum intensity projection along the first axis of a image 
    provided as numpy array and returns the result as numpy array.
    
        
* [mean_squared_error](mean_squared_error.ipynb): 
    Takes two images provided as numpy arrays and returns the mean-squared-error of the two images compared pixel-by-pixel.
    
        
* [mean_std_column](mean_std_column.ipynb): 
    Computes the mean average and standard deviation of a column specified by name 
    in a given dataframe and returns these two numbers as tuple.
    
        
* [measure_aspect_ratio_of_regions](measure_aspect_ratio_of_regions.ipynb): 
    Takes a label image provided as numpy array and returns a pandas dataframe
    with a column containing measurements for aspect_ratio of the objects.
    
        
* [measure_intensity_of_labels](measure_intensity_of_labels.ipynb): 
    Takes a label image and an intensity image, and returns a list of mean intensities 
    of all pixels in the intensity image, belonging to a given label.
    
        
* [measure_intensity_over_time](measure_intensity_over_time.ipynb): 
    Takes a timelapse (list of images provided as numpy arrays), 
    measures the average intensity in the images over time and 
    returns the resulting measurements as list.
    
        
* [measure_mean_image_intensity](measure_mean_image_intensity.ipynb): 
    Takes an image provided as numpy array and returns its mean intensity.
    
        
* [measure_pixel_count_of_labels](measure_pixel_count_of_labels.ipynb): 
    Takes a label image provided as numpy array and returns a list of counts of number of pixels per label.
    
        
* [measure_properties_of_regions](measure_properties_of_regions.ipynb): 
    Takes a label image and an intensity image, both provided as numpy array, 
    and returns pandas dataframe with measurements for area, perimeter and 
    mean_intensity of the labeled objects.
    
        
* [open_image_read_voxel_size](open_image_read_voxel_size.ipynb): 
    Reads an image file as specified by filename and return the voxel size of the image as (Z,Y,X) tuple.
    
        
* [open_image_return_dimensions](open_image_return_dimensions.ipynb): 
    Opens an image specified by filename and returns its dimensions as (height, width) tuple.
    
        
* [open_nifti_image](open_nifti_image.ipynb): 
    This function loads a nifti image from the specified filename image_file_location and returns the image data as a numpy array. 
    
        
* [open_zarr](open_zarr.ipynb): 
    Opens a zarr file as specified by filename zarr_file_location and returns the data as numpy array
    
        
* [pair_wise_correlation_matrix](pair_wise_correlation_matrix.ipynb): 
    Takes a pandas dataframe and computes for all columns their Pearson's correlation coefficient
    for all columns in the dataframe. For n columns, this is a n x n matrix of coefficients.
    The matrix is returned as dataframe.
    
        
* [radial_intensity_profile](radial_intensity_profile.ipynb): 
    returns the radial intensity profile as list of numbers from an 
    image provided as numpy array around a given 2d coordinate specified as xc, yc. 
    
        
* [region_growing_segmentation](region_growing_segmentation.ipynb): 
    Segments an image provided as numpy array using the region-growing algorithm 
    (sometimes called flood-filling algorithm) starting from a single point provided as y-x tuple. 
    Returns the resulting segmentation binary image as numpy array.
    
        
* [remove_labels_on_edges](remove_labels_on_edges.ipynb): 
    Takes a label_image given as numpy array, removes all objects which touch the image border
    and returns the resulting label image.
    
        
* [remove_noise_edge_preserving](remove_noise_edge_preserving.ipynb): 
    Applies an edge-preserving noise-removal filter with a given radius to an 
    image provided as numpy array and returns the filtered image as numpy array.
    
        
* [remove_small_labels](remove_small_labels.ipynb): 
    Takes a label_image provided as nump array, removes all objects that are smaller than a given size_threshold 
    and returns the resulting label image as numpy array.
    
        
* [return_hello_world](return_hello_world.ipynb): 
    Returns the string "hello world".
    
        
* [rgb_to_grey_image_transform](rgb_to_grey_image_transform.ipynb): 
    Convert an RGB image provided as numpy array with the third dimension being the color
    to a single-channel gray scale image with configurable weights r, g and b.
    The weights are normalized to be 1 in sum.
    The resulting single-channel image is returned as numpy array.
    
        
* [rotate_image_by_90_degrees](rotate_image_by_90_degrees.ipynb): 
    Rotates an image provided as numpy array by 90 degrees clockwise around the center of the image and 
    returns the resulting image as numpy array.
    
        
* [subsample_image](subsample_image.ipynb): 
    Subsamples a 2D image provided as numpy array by skipping every n'th pixel in X and Y and 
    returns the resulting numpy array.
    
        
* [subtract_background_tophat](subtract_background_tophat.ipynb): 
    Applies a top-hat filter with a given radius to an image provided as numpy array with 
    dark background (low values) and bright foreground (high values). The resulting 
    background-subtracted image is returned as numpy array.
    
        
* [sum_images](sum_images.ipynb): 
    Sums two images pixel-by-pixel and returns the result.
    All input images and also the result image are of type numpy array.
    
        
* [sum_intensity_projection](sum_intensity_projection.ipynb): 
    Performs a maximum intensity projection along the first axis of an image provided as numpy array.
    The resulting image is returned as numpy array.
    
        
* [tiled_image_processing](tiled_image_processing.ipynb): 
    Applies a maximum filter with a given radius to the image provided as numpy-array using a tile-by-tile strategy.
    The tile_size denotes the size of the tiles in X and Y.
    The resulting, re-assembled image is returned as numpy array.
    
        
* [transpose_image_axes](transpose_image_axes.ipynb): 
    Transposes the first two axes of an image and returns the result.
    Input image and returned result image are numpy arrays.
    
        
* [t_test](t_test.ipynb): 
    Takes a dataframe and two column names to apply a paired T-test to the two columns to determine and return the p-value.
    
        
* [workflow_batch_process_folder_count_labels](workflow_batch_process_folder_count_labels.ipynb): 
    This functions goes through all .tif image files in a specified folder full of label images, 
    loads the label images and counts unique labels in each image. 
    It returns a dictionary with filenames as keys and corresponding counts as values.
    
        
* [workflow_batch_process_folder_measure_intensity](workflow_batch_process_folder_measure_intensity.ipynb): 
    This functions goes through all .tif image files in a specified image folder 
    and corresponding label images in another labels folder. 
    It loads the images and corresponding label images, and measures minimum, mean and maximum intensity of all labeled objects.
    The function returns a dataframe with five columns: min_intensity, mean_intensity, max_intensity, label and filename.
    
        
* [workflow_segmentation_counting](workflow_segmentation_counting.ipynb): 
    This function segments objects in an image provided as numpy array with intensity above average 
    and returns their count as number.
    
        
* [workflow_segmentation_measurement_summary](workflow_segmentation_measurement_summary.ipynb): 
    This function implements a workflow consisting of these steps:
    * threshold intensity input image provided as numpy array using Otsu's method
    * label connected components
    * measure area of the labeled objects
    * determine mean area of all objects and return it
    
        
* [workflow_segment_measure_umap](workflow_segment_measure_umap.ipynb): 
    This function takes a single channel intensity image provided as numpy array, 
    segments objects with intensity above half the maximum intensity, 
    labels connected components, 
    measures area, perimeter, mean_intensity, minor and major axis of the labeled objects, 
    and produces a UMAP from the given measurements. 
    The two UMAP vectors are saved as `umap0` and `umap1` togther with the measurements in a dataframe. 
    The function returns this dataframe.
    
        
* [workflow_watershed_segmentation_correction_measurement](workflow_watershed_segmentation_correction_measurement.ipynb): 
    This function implements a workflow consisting of these steps:
    * Gaussian blur an image provided as numpy array with a sigma of 1
    * detect local minima in the blurred image
    * apply watershed segmentation flooding the blurred image from the 
      detected minima to retrieve a label image
    * remove all objects which touch the image border
    * measure the area of all remaining objects together and return it
    
        