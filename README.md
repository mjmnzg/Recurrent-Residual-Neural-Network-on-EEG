# Cross-subject classification of cognitive loads using a recurrent-residual deep network

Abstract: The problem of automatically learning temporal and spectral feature representations for EEG signals has been intensely studied in the last years. However, most solutions are focused on extracting representations used for training classifiers in particular subjects. This is not well suitable for applications involving several subjects, since it requires high computing times and costs at labeling data and training classifiers for each new subject involved. To address this problem, we propose an improvement of a deep neural network architecture, using residual layers and Gated Recurrent Units (GRU), able to extract feature representations for “cross-subject” classification. Our architecture, called RecResNet, achieved a better accuracy (0.907±0.124) and F-measure (0.896±0.148) than other baseline methods, when applied to the classification of four levels of cognitive loads using 13 subjects.

	

Please consider citing our paper if you find this code useful in your research:
	
	@INPROCEEDINGS{Recresnet2017, 
		author={M. {Jiménez-Guarneros} and P. {Gómez-Gil}}, 
		booktitle={2017 IEEE Symposium Series on Computational Intelligence (SSCI)}, 
		title={Cross-subject classification of cognitive loads using a recurrent-residual deep network}, 
		year={2017}, 
		pages={1-7}, 
		doi={10.1109/SSCI.2017.8280897}, 
		month={Nov}}

Link: https://ieeexplore.ieee.org/document/8280897


Packages:

	- Python (>= 3.6)
	- Tensorflow (>= 1.9)
	- NumPy (>= 1.8.2)
	- SciPy (>= 0.13.3)

Command to execute project:

	CUDA_VISIBLE_DEVICES=0 python3 run_main.py --model resrecnet --dataset pbashivan --output outputs/resrecnet
