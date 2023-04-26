# FeDG

Usage
Start with a demo for continuous frequency space interpolation among federated clicnets:
python freq_space_interpolation_demo.py


Prepare the dataset, and then extract the amplitude spectrum of samples in each local client with the function in dataset/prepare_dataset.py:

Organize the data (save the data as npy to speed up federated training) and amplitude spectrum of local clients as following structure:

  ├── dataset
     ├── client1
        ├── data_npy
            ├── sample1.npy, sample2.npy, xxxx
        ├── freq_amp_npy
            ├── amp_sample1.npy, amp_sample2.npy, xxxx
     ├── clientxxx
     ├── clientxxx
     
Train the federated learning model with ELCFS:

python train_ELCFS.py
