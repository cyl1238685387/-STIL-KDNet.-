# STIL-KDNet

Abstract—In the task of remote sensing image change detection
and segmentation, accurately identifying and segmenting changed
regions is crucial for surface dynamic monitoring. Current meth-
ods, when dealing with complex scenarios, have limited detection
and segmentation accuracy due to difficulties in capturing spatio-
temporal feature differences. To address this, this paper proposes
an innovative method to enhance the model’s capabilities. First,
a perturbation set is obtained by perturbing Image B. Then, the
original dual-temporal image set and the perturbation set are
input into the backbone network for training. Meanwhile, knowl-
edge distillation is introduced, with the original set as the teacher
model and the perturbation set as the student model. The original
supervised loss, the student’s distillation loss, and the supervised
loss are combined, and a specially designed loss function is used to
measure the output differences between the teacher and student
models. During change detection and segmentation, minimizing
this function and back-propagating the three losses optimize the
network parameters, enabling the student model to fit the teacher
model’s output distribution, calibrate its predictions to approach
the teacher model’s judgment logic, and improve performance,
providing accurate results for surface monitoring. Experiments
show that this lightweight network has excellent accuracy and
efficiency on the LEVIR-CD,SYSU-CD,and WHU-CD datasets.
![image](https://github.com/user-attachments/assets/86ced9e3-e35c-4802-9e17-2b60c2c74373)
