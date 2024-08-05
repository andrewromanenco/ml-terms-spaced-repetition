#image

The intersection of two sets divided by their union. In machine-learning
image-detection tasks, IoU is used to measure the accuracy of the model&#39;s
predicted [[bounding box|bounding box]] with respect to the
[[ground truth|ground-truth]] bounding box. In this case, the IoU for the
two boxes is the ratio between the overlapping area and the total area, and
its value ranges from 0 (no overlap of predicted bounding box and ground-truth
bounding box) to 1 (predicted bounding box and ground-truth bounding box have
the exact same coordinates).

For example, in the image below:

<ul>
<li>The predicted bounding box (the coordinates delimiting where the model
predicts the night table in the painting is located) is outlined in purple.</li>
<li>The ground-truth bounding box (the coordinates delimiting where the night
table in the painting is actually located) is outlined in green.</li>
</ul>


![[ images/iou_van_gogh_bounding_boxes.jpg ]]


Here, the intersection of the bounding boxes for prediction and ground truth
(below left) is 1, and the union of the bounding boxes for prediction and
ground truth (below right) is 7, so the IoU is \(\frac{1}{7}\).

<div id="intersection-union-side-by-side">
![[ images/iou_van_gogh_intersection.jpg ]]

![[ images/iou_van_gogh_union.jpg ]]
</div>

