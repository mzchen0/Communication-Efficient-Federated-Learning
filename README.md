# Communication-Efficient-Federated-Learning
Pleasue use Matlab 2018b or above to run the simulations.

The simulations consist of three main files: MINST,CIFAR, and Finger movement detection.

To run MINST, one must first download the MINST dataset. Then, one can run the code MIN-CPU.m or MIN-GPU.m.

CIFAR is used for image identification. Before running the code CIFAR.m, one must first run the code DownloadCIFAR10.m to downlowd the dataset of CIFAR. After that, one must run the code 

% if ~exist('cifar10Train','dir')\\
%     disp('Saving the Images in folders. This might take some time...');   \\ 
%     saveCIFAR10AsFolderOfImages('cifar-10-batches-mat', pwd, true);\\
% end

to classify the CIFAR dataset. Then, one can directly run the code CIFAR.m. 

For finger movement detection, we have include the data that has been processed by window method. Therefore, one can directly run the code FMD.m.

In coding setting, stSettings.type determine the coding method. For example, stSettings.type=2 implies that Dithered 2-D lattice quantization method is used for coding while stSettings.type=3 implies that Dithered scalar quantization is used for coding. s_fRate determines the number of bits used to represent one element in the local FL model vector.
