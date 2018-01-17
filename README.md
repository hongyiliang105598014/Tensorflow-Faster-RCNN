./tools/train_net.py --device gpu --device_id 0 --weight data/pretrain_model/VGG_imagenet.npy --imdb voc_2007_trainval --iters 70000 --cfg experiments/cfgs/faster_rcnn_end2end.yml --network VGGnet_train

./tools/test_net.py --device gpu --device_id 0 --weight output/faster_rcnn_end2end/voc_2007_trainval/VGGnet_fast_rcnn_iter_70000.ckpt --imdb voc_2007_test --cfg experiments/cfgs/faster_rcnn_end2end.yml --network VGGnet_test

im_detect: 4952

AP for bicycle = 0.7857
AP for bus = 0.7712
AP for car = 0.7968
AP for motorbike = 0.7417
AP for person = 0.7488
AP for train = 0.7524
Mean AP = 0.7661
~~~~~~~~
Results:
0.786
0.771
0.797
0.742
0.749
0.752
0.766
~~~~~~~~
