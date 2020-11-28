# To do:
1. Train an AlexNet classifier on CIFAR-10 in Tensorflow or PyTorch.
2. Train two separate linear SVM classifiers on training data embeddings extracted from two different intermediate locations of the AlexNet network.
3. Report the performances of vanilla AlexNet and the two SVM classifiers on the CIFAR-10 test data.

# Result insights:
1. The models, as of now, has regularization issues where training data accuracies are ~90%, whereas the test data accuracies are ~65%.
    - Additional data augmentation tasks for creating additional rotated/translated data has not been included, which might help with better performance and generalization, as of now.
2. As for the performance comparison of vanilla AlexNet vs Linear SVM using intermediate embeddings from AlexNet, we see that the training performances are not that significantly different. However, the AlexNet seems to have marginally better testing performance compared to the SVMs.
    - The SVMs used are multi-class LinearSVC with One-vs-Rest model instead of One-vs-One model.
 
