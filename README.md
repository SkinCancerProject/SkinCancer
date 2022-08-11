# DESIGN OF A TOOL FOR THE CLASSIFICATION OF SKIN CANCER IMAGES IN AN ANDROID SYSTEM.

This repository belongs to the public research carried out by Duván González and Sebastián Rivera, which is based on the application of the knowledge distillation technique for the classification of the three skin cancers with the highest incidence, this project was carried out in the research modality of undergraduate degree for the degree of professional engineer.

DISEÑO DE UNA HERRAMIENTA PARA LA CLASIFICACIÓN DE IMÁGENES DE CÁNCER DE PIEL EN UN SISTEMA ANDROID

El cáncer de piel pertenece a los diez tipos de cáncer más comunes que se registran en todo el mundo. Según la OMS, en 2020 se registraron más de un millón de casos (distintos del melanoma). Esta es una preocupación latente, ya que su crecimiento continúa y su diagnóstico puede ser demorado, o en algunos casos, inexistente para personas carentes de un sistema de salud. Hoy en día, las redes neuronales permiten una clasificación de imágenes con gran probabilidad de éxito. Es por esta razón, que en esta investigación se diseña una herramienta que permita clasificar imágenes de cáncer de piel en un sistema Android. Tomando como punto de partida el trabajo realizado por Diana Merchán y Helis Navarro se aplicó una técnica conocida como destilación del conocimiento. Esta técnica permite que este modelo actúe como Teacher y destile o entregue sus conocimientos a una red conocida como Student. Además, la red del Student se formó mediante redes neuronales residuales que permiten agregar saltos entre sus capas con el fin que el gradiente no se desvanezca al realizar el backpropagation. Estas técnicas se usaron para comprimir el modelo y mantener o mejorar su rendimiento. Se pasó de tener un rendimiento de 0.9332 a 0.9557 (puntuación F1 Score) para la clasificación entre imágenes cancerígenas de tipo Benigno v.s Maligno. Además, se logró una compresión del 96.75\% del modelo Teacher respecto al modelo del $student$. Estos resultados fueron obtenidos haciendo un ajuste fino en los hiperparámetros y seleccionando los mejores que son: K=3, alpha=0.2 y T=1. También se usaron estas técnicas para una entrada de tres clases, pasando de un rendimiento de 0.7815 para la red del $teacher$ a 0.8995 para la red $student$. A su vez, se logró una compresión del 95.71\% del modelo Student respecto al modelo Teacher. Estos resultados para una entrada de tres clases se lograron con los hiperparámetros: K=4, alpha=0.3 y T=5. Finalmente, los dos mejores modelos correspondientes a cada tipo de entrada, fueron implementados en un sistema Android donde se puede tomar o cargar una foto y hacer su respectiva inferencia.


#REFERENCIAS

[1] OMS, “C ́ancer.” [En l ́ınea]. Disponible: https://www.who.int/es/news-room/fact-sheets/detail/cancer
[2] D. P. M. Vargas, H. N. B ́aez, J. G. B. P ́erez, and J. A. C. Boh ́orquez, “Design of a tool for the classification of skin cancer images using deep
neural networks (dnn),” Ciencia y Tecnolog ́ıa, pp. 65–80, 2021.
[3] M. F. for Medical Education and Research, “C ́ancer de piel,” 2020. [En l ́ınea]. Disponible: https://www.mayoclinic.org/es-es/diseases-conditions/skin-cancer/symptoms-causes/syc-20377605
[4] M. de Salud y Protecci ́on Social, “Manual para la prevenci ́on del c ́ancer de piel no melanoma dirigido al entorno educativo,” 2015. [En l ́ınea]. Disponi-
ble: https://www.minsalud.gov.co/sites/rid/Lists/BibliotecaDigital/RIDE/VS/PP/ENT/manual-prevencion-cancer-piel-entorno-educativo.pdf
[5] L. C. C. el C ́ancer, “Datos—c ́ancer de piel,” 2021. [En l ́ınea]. Disponible: https://www.ligacancercolombia.org/educacion/datos-cancer-de-piel/
[6] A. M. de Bogot ́a D.C, “Ley 1384 de 2010 nivel nacional,” 2010. [En l ́ınea]. Disponible: https://www.alcaldiabogota.gov.co/sisjur/normas/Norma1.jsp?i=39368
[7] M. de Salud y Protecci ́on Social, “Vicesalud destac ́o acciones de colombia frente al c ́ancer de piel,” 2020. [En l ́ınea]. Disponible: https://www.minsalud.gov.co/Paginas/Vicesalud-destaco-acciones-de-Colombia-frente-al-cancer-de-piel.aspx
[8] M. y. E. A. Instituto de Hidrolog ́ıa, “Escenarios de cambio climático,” 2015. [En l ́ınea]. Disponible: http://www.ideam.gov.co/web/tiempo-y-clima/escenarios-cambio-climatico
[9] C. D. S. Machado Filho, D. S. Fagundes, F. Sender, G. L. Saraiva,L. H. C. Paschoal, M. C. C. d. Costa, R. M. E. Cunha, and S. G.
Carazzato, “Neoplasias malignas cutˆaneas: estudo epidemiol ́ogico,” An.bras. dermatol, pp. 479–84, 1996.
[10] J. R. Ana Francisca Ram ́ırez, Juan Guillermo Chalela, “¿cu ́antos dermat ́ologos hay en colombia? an ́alisis de los datos de la
asociaci ́on colombiana de dermatolog ́ıa y cirug ́ıa dermatol ́ogica,” 2012. [En l ́ınea]. Disponible: https://revistasocolderma.org/sites/default/files/cuantos dermatologos hay en colombia.pdf
[11] A. N. Hoshyar, A. Al-Jumaily, and R. Sulaiman, “Review on automatic early skin cancer detection,” in 2011 International Conference on
Computer Science and Service System (CSSS). IEEE, 2011, pp. 4036–4039.
[12] J. M. Haglin, G. Jimenez, and A. E. Eltorai, “Artificial neural networks in medicine,” Health and Technology, vol. 9, no. 1, pp. 1–6, 2019.
[13] A. Esteva, B. Kuprel, R. A. Novoa, J. Ko, S. M. Swetter, H. M. Blau,and S. Thrun, “Dermatologist-level classification of skin cancer with
deep neural networks,” nature, vol. 542, no. 7639, pp. 115–118, 2017.
[14] H. Alquran, I. A. Qasmieh, A. M. Alqudah, S. Alhammouri, E. Alawneh,A. Abughazaleh, and F. Hasayen, “The melanoma skin cancer detection
and classification using support vector machine,” in 2017 IEEE JordanConference on Applied Electrical Engineering and Computing Techno-
logies (AEECT). IEEE, 2017, pp. 1–5.11
[15] T. J. Brinker, A. Hekler, J. S. Utikal, N. Grabe, D. Schadendorf, J. Klode,C. Berking, T. Steeb, A. H. Enk, and C. Von Kalle, “Skin cancer
classification using convolutional neural networks: systematic review,”Journal of medical Internet research, vol. 20, no. 10, p. e11936, 2018.
[16] D. P. M. Vargas, H. N. B ́aez, J. G. B. P ́erez, and J. A. C. Boh ́orquez,“Design of a tool for the classification of skin cancer images using deep
neural networks (dnn),” Ciencia y Tecnolog ́ıa, pp. 65–80, 2021.
[17] Google, “Using ai to help find answers to common skin conditions,”2021. [En l ́ınea]. Disponible: https://blog.google/technology/health/ai-dermatology-preview-io-2021/
[18] I. Archive, “Skin cancer isic.” [En lınea]. Disponible: https://www.isic-archive.com/#!/topWithHeader/wideContentTop/main
[19] S. R. Duvan Gonz ́alez, “Skincancerproject/skincancer,” 2022. [En lınea]. Disponible: https://github.com/SkinCancerProject/SkinCancer
[20] K. He, X. Zhang, S. Ren, and J. Sun, “Deep residual learning for image recognition,” CoRR, vol. abs/1512.03385, 2015. [En lınea]. Disponible:
http://arxiv.org/abs/1512.03385
[21] L. Tarr ́es Benet, “Clasificaci ́on de lesiones en la piel con un ensemble de redes neuronales residuales,” B.S. thesis, Universitat Politecnica de
Catalunya, 2019.
[22] J. A.-T. Barrera, “Redes neuronales,” Universidad de Guadalajara Disponible en: http://www. cucei. udg.mx/sites/default/files/pdf/toral barrera jamie areli. pdf [Visitada en octubre de 2016].
[23] L. Team, “Deep learning de la a - z: Redes neuronales en python desde cero,” Udemy [Curso Virtual] Disponible en: https://www.udemy.com/course/deep-learning-a-z/. Visitada en Junio de 2022.
[24] C. Buciluˇa, R. Caruana, and A. Niculescu-Mizil, “Model compression,” in Proceedings of the 12th ACM SIGKDD international conference on
Knowledge discovery and data mining, 2006, pp. 535–541.
[25] G. Hinton, O. Vinyals, and J. Dean, “Distilling the knowledge in a neural network,” 2015. [En lınea]. Disponible: https://arxiv.org/abs/1503.02531
[26] Keras, “Knowledge distillation.” [En lınea]. Disponible: https://keras. io/examples/vision/knowledge distillation/
[27] J. Gou, B. Yu, S. J. Maybank, and D. Tao, “Knowledge distillation: A survey,” International Journal of Computer Vision, vol. 129, no. 6, pp.
1789–1819, 2021. 
[28] S. Overflow, “What is the meaning of the word logits in tensorflow? [duplicate],” 2017. [En lınea]. Disponible: https://stackoverflow.com/questions/41455101/what-is-the-meaning-of-the-word-logits-in-tensorflow
[29] J. Korstanje, “The f1 score,” 2021. [En lınea]. Disponible: https: //towardsdatascience.com/the-f1-score-bec2bbc38aa6
[30] C. A. Fajardo, A. S. Parra, T. V. Castellanos Parada, and K. Roy, “Towards atrial fibrillation detection in wearable devices using deep
learning.”
[31] T. Lite, “Deploy machine learning models on mobile and edge devices.” [En l ́ınea]. Disponible: https://www.tensorflow.org/lite?hl=es-419
[32] A. Studio, “Android for developers.” [En lınea]. Disponible: https://developer.android.com/
[33] Canva, “Canva.” [En lınea]. Disponible: https://www.canva.com/es us/
[34] storyset, “Ilustraci ́on del concepto de melanoma.” [En lınea]. Disponible: https://www.freepik.es/vector-gratis/ilustracion-concepto-melanoma25923174.htm#page=4&query=skin%20cancer&position=28&fromview=search
[35] RawPixel, “Maqueta de pantalla de tel ́efono inteligente, ilustraci ́on de vector de dispositivo digital.” [En lınea]. Disponible: https://www.freepik.es/vector-gratis/maqueta-pantalla-telefono-inteligente-ilustracion-vector-dispositivo-digital19085884.htm#page=2&query=celular%20en%20la%20mano&position=31&fromview=search
[36] P. Velasquez, “https://consultorsalud.com/cancer-de-piel-como-esta-colombia-en-esta-materia/,” 2020. [En lınea]. Disponible: https://consultorsalud.com/cancer-de-piel-como-esta-colombia-en-esta-materia/


