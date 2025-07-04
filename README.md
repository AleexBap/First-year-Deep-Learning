# Project Report 🕵️

## Institution:
Master in Data Science, Faculdade de Ciências da Universidade de Lisboa, Portugal.

## Title: Car Damage and Repair Cost Estimation Using Image Segmentation

### Abstract:
Accurate vehicle damage assessment is fundamental for automotive industries to manage insurance claims and repair pricing, yet this process still often depends on manual, on-site inspections that are time-consuming, costly, and prone to human subjectivity.
Some early digital solutions are being developed, showing that deep learning can detect damage in images and provide repair estimate, however these tools remain largely unused by insurers, only cover a few and frequent classes (scratch, dent, crack) often miss and omit rare damage patterns, and it ignores the size and severity of each instance therefore it does not translate detection into a reliable repair cost estimates. This limitation leaves a clear gap for a finer-grained, per-damage system that scales to more categories and adjusts cost to the actual extent of each defect.
To address this gap, we aim to build a YOLOv8-based segmentation pipeline that can turn a customer-supplied photo into a structured damage report. The system detects and masks multiple exterior damages, classifies their type and severity, and provides an appropriate repair-cost range. Using the Car Damage Severity Detection (CarDD) dataset extracted in YOLOv8 format, that allows multi-label polygon masks per image, three main experiments were conducted: (1) hyper-parameter search on the balanced YOLOv8m-seg baseline, (2) impact of augmentation, and (3) model-size comparison (s, m, l) across 10–50 epochs.
We found that the best performer, YOLOv8-l-seg at 50 epochs, reached mAP50 = 0.45 for bounding boxes and 0.44 for masks, delivering accurate and consistent detection. These results confirm the feasibility of rapid, photo-based damage triage that reduces on-site inspection costs and improves claim cost estimations. Remaining challenges include class imbalance and translating mask geometry into precise costs. Future work will add a regression head that leverages mask size, location and learned severity cues to output a per-damage repair-cost range.

## Contributors: https://github.com/Princesacorderosa

## Teacher: Nuno Cruz Garcia

https://ncgarcia.github.io

## Grade for the hole project:  16,6/20,0
