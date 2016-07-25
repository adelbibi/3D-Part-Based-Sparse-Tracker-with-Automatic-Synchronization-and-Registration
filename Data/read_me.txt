%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
	3D Part-Based Sparse Tracker with Automatic Synchronization and Registration
				Adel Bibi, Tianzhu Zhang, and Bernard Ghanem
		King Abdullah University of Science and Technology (KAUST), Saudi Arabia
			{adel.bibi,tianzhu.zhang,bernard.ghanem}@kaust.edu.sa
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

Some videos require Registration only, other require Synchronization, and some require both jointely.

The videos are from the Princeton RGBD benchmark[2,3].
1) For any video that requires registration, a folder named "registered_depth" can be found where manual registration with
RGB images have been conducted. Keep in mind the registration is not global but rather local on the target being tracked.

2) As for the videos that require syncrhonization, a .mat file named "FrameID_sync" indicated the proper ordering of the depth sequence
to match the RGB sequence.

3) As for videos that require both, the .mat file "Frame_sync" indicate the order in which the depth stream from the "registered_depth" has to be
read in.


The list of videos follows:

Videos that need only Registeration:

    'basketball1'
    'basketball2'
    'book_move1'
    'new_ex_no_occ'
    'new_student_center4'
    'new_student_center_no_occ'
    'studentcenter2.1'
    'studentcenter3.2'
    'basketball2.2'
    'toy_mo_occ'
    'toy_no'
    'toy_no_occ'
    'two_book'
    'zballpat_no1'


Videos that need only Syncrhonization:

    'bear_back'
    'cafe_occ1'
    'cf_occ2'
    'cf_occ3'
    'dog_occ_3'
    'hand_no_occ'
    'new_ex_occ1'
    'new_ex_occ6'
    'new_ex_occ7.1'
    'rose1.2'
    'static_sign1'
    'toy_car_occ'
    'wr_no'

Videos that need both:

    'cup_book'
    'library2.1_occ'
    'new_student_center1'
    'new_student_center2'
    'new_student_center3'
    'studentcenter3.1'
    'walking_no_occ'
    
    
    Referrences:
    [1] "3D Part-Based Sparse Tracker with Automatic Synchronization and Registration", Computer Vision and Pattern Recognition (CVPR16).
    [2] "Tracking Revisited using RGBD Camera: Unified Benchmark and Baselines", IEEE International Conference on Computer Vision (ICCV2013)
    [3] http://tracking.cs.princeton.edu
