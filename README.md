# "Effects of Pose Normalization on Weakly Supervised 3D Human Pose Estimation"
This is the Bachelor's thesis I wrote for my B.Sc. degree in Computer Science during the summer term 2019.
It is about the effects of pose normalization in the 2D-to-3D-Pose-Estimation system proposed by Drover et al. [1].

The following are the abstracts in English and German:

## Abstract
With well-performing 2D human pose estimators evolving over the last years, recent work focuses on inferring 3D poses from 2D poses.
During the ECCV 2018 Workshops, Drover et al. presented such a 2D to 3D pose estimator in their work "Can 3D Pose be Learned from 2D Projections Alone?".
Using a Generative Adversarial Network, their system is able to achieve state of the art results.
On top of that, its main feature is that no 3D ground truth poses are required for training, which makes it especially attractive in applications where no ground truth data is available.

In their proposed system, Drover et al. require the 2D input poses to be normalized in scale and position.
The goal of this thesis is to analyze the effects of this normalization on the qualitative performance of the 3D pose estimation in that system.
For this, baseline results for synthetically generated poses are established in a first step.
Subsequently, the effects of normalization in position and scale are analyzed.
Both the theoretical findings and the conducted experiments show that the normalization indeed negatively influences the measurable error.
Since especially the normalization in position accounts for a significant increase in error, the system is modified to compensate for this.

In addition to the analysis of the effects of normalization, an alternative loss function is proposed.
It leverages high-level knowledge about the structure of human poses to produce improved results.
With this new loss function, the error can be reduced by more than 7%. 

## Zusammenfassung
Da in den letzten Jahren leistungsstarke 2D Posenerkennungssysteme entwickelt wurden, liegt der Fokus jüngster Forschung darauf, aus diesen 2D Posen 3D Posen zu generieren.
Während den ECCV 2018 Workshops haben Drover et al. in ihrer Arbeit "Can 3D Pose be Learned from 2D Projections Alone?" (in etwa "Können 3D Posen ausschließlich von 2D Projektionen erlernt werden?") ein solches System vorgestellt, das für menschliche 2D Posen die dazugehörigen 3D Posen generiert.
Mit Hilfe eines Generative Adversarial Networks gelingt es diesem System Ergebnisse zu erzielen, die dem aktuellen Stand der Technik entsprechen.
Darüberhinaus bietet das System den großen Vorteil, dass für das Training keine 3D Grundwahrheitsposen benötigt werden.
Dies macht das System besonders für Anwendungen attraktiv, in denen keine Grundwahrheitsdaten vorhanden sind.

In dem von Drover et al. vorgestellten System müssen die 2D Eingabeposen in Größe und Position normalisiert sein.
Das Ziel dieser Arbeit ist es, die Effekte dieser Normalisierung auf die qualitative Leistungsfähigkeit der 3D-Posengenerierung zu analysieren.
Dafür werden als Erstes Ausgangsresultate für synthetisch generierte Posen ermittelt.
Anschließend werden die Effekte der Größen- und Positionsnormalisierung analysiert.
Sowohl die theoretische Untersuchung als auch die durchgeführten Experimente zeigen, dass die Normalisierung den messbaren Fehler negativ beeinflusst.
Da insbesondere die Größennormalisierung für einen deutlichen Anstieg des Fehlers verantwortlich ist, wird das System so modifiziert, dass der dadurch verursachte Fehler kompensiert wird.

Zusätzlich zur Analyse der Effekte der Posennormalisierung wird eine alternative Fehlerfunktion vorgestellt.
Diese verwendet allgemeines Wissen über die Struktur menschlicher Posen, um verbesserte Ergebnisse zu erzielen.
Mit der neuen Fehlerfunktion kann der Fehler um mehr als 7% reduziert werden. 


## References
[1] Dylan Drover, Rohith M. V, Ching-Hang Chen, Amit Agrawal, Ambrish Tyagi, and Cong Phuoc Huynh. Can 3D Pose Be Learned from 2D Projections Alone?
  In Computer Vision – ECCV 2018 Workshops, pages 78–94. Springer International
  Publishing, 2019
