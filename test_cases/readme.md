
# List of use-cases
This list of 76 use-cases is auto-generated. Do not modify this file.


* [apply_otsu_threshold_and_count_positive_pixels](apply_otsu_threshold_and_count_positive_pixels.ipynb): 
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
    
        
* [create_polygon_from_coordinates](convert_points_polygon.ipynb): 
    Take a list of 4 or more coordinates in xy format and convert it into a shapely polygon. Return the polygon.
    
        
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
    
        
* [None](create_multipolygon_from_coordinates.ipynb): 
    Take a list of coordinate lists that intersect only at one point and create a shapely multipolygon. 
    The multipolygon must be valid. Return the multipolygon
    
        
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
    
        
* [detect_ellipse](detect_ellipse.ipynb): 
    Given a binary edge map, detect the ellipse in the image using a Hough Transform.
    Return the center of the ellipse in the image as a tuple (y, x).
    
        
* [distance_between_maxima](distance_between_maxima.ipynb): 
    Takes two images as input, finds the maximum pixel in each image, and returns 
    the distance in pixels between the two maxima.
    Input: two 2D images as separate inputs
    Output: Float
    
        
* [expand_labels_without_overlap](expand_labels_without_overlap.ipynb): 
    Takes a label_image and enlarges all labels by a given radius, without
    labels overwriting each other.
    
        
* [extract_surface_measure_area](extract_surface_measure_area.ipynb): 
    Take a 3D binary_volume_image, extracts the surface of the white (voxel value != 0) object 
    and returns the surface area of the object.
    
        
* [fft_spectrum](fft_spectrum.ipynb): 
        Returns the FFT spectrum of an arbitrary nD image as the absolute logarithm (log1p) of the Fourier transform magnitude. Ensures that the DC component is at the center of the image. Uses reflection padding (provided as integer parameter) and Hamming apodization to reduce artefacts due to discontinuities at the image borders.
        
        
* [find_closest_neighbors](find_closest_neighbors.ipynb): 
    Given a label_image and target_label number of interest, find the n closest 
    other labelled regions (by inter-centroid distance) and return them as list
    
        
* [fit_circle](fit_circle.ipynb): 
    Implements 2D circle fitting
    Input: Collection of 2d points, represented as a list of lists [ [x0,y0], [x1,y1], ... ]  
    Output: Tuple: xc, yc, radius
    
        
* [fit_gaussian_to_spot](fit_gaussian_to_spot.ipynb): 
    Implements 2D gaussian fitting to a noisy spot in the image, find the center (xc, yc) and 
    standard deviation (sigma) of the gaussian fit to the spot, all in pixel coordinates. 
    Perform the fit using unweighted least-squares fitting, in which the sum of squared errors in minimized.
    The first pixel (top-left corner) has coordinates (0,0). Background knowledge: the 
    image contains a single noisy gaussian spot with a width of approximately 5 pixels. 
    The intensity of the spot and number of background photons is arbitrary. 
    The pixel size is irrelevant, since everything is in pixel units.

    Input: 2D square grayscale image
    Output: Tuple: (xc, yc, sigma)
    
        
* [flow_field_deformation](flow_field_deformation.ipynb): 
    Given a vector field `flow_field` (H, W, 2) in which every pixel represents the relative 
    displacement vector to its position, then apply the deformation to the target (N, W) 
    image and return the deformed image.
    
        
* [generate_image_histogram](generate_image_histogram.ipynb): 
    Takes a 2D input image, generates a histogram of the image using the value in num_bins and returns only the histogram values
    
        
* [identify_centroids](identify_centroids.ipynb): 
    Given a label image, return a dict of {label: [list of weighted floating-point centroid coords], ...}  for each labelled
    region (assume contiguity). Labels run between 1 and some integer n.
    
        