## Laporan Interpretasi Hasil
Network pharmacology pada penyakit atherosclerosis dilakukan dengan pendekatan multi-komponen–multi-target menggunakan enam senyawa bioaktif, yaitu quercetin, wogonin, β-sitosterol, baicalein, (R)-canadine, dan berberine. Pendekatan ini bertujuan mengidentifikasi interaksi senyawa dengan berbagai target protein dan jalur biologis yang berperan dalam patogenesis aterosklerosis melalui analisis jaringan, GO, KEGG, dan molecular docking (Xie et al., 2020; Ji et al., 2023).  Proses ini dimulai dari identifikasi struktur senyawa melalui PubChem, kemudian dilakukan prediksi target protein menggunakan SwissTargetPrediction. Langkah awal ini menjadi dasar untuk menghubungkan senyawa dengan target molekuler yang relevan terhadap penyakit. Selanjutnya, gen/protein yang berasosiasi dengan atherosclerosis dikumpulkan dari basis data seperti OMIM, lalu dicari irisan dengan target senyawa untuk memperoleh kandidat target potensial. Tahap irisan ini penting karena menyaring target yang benar-benar relevan dengan patogenesis atherosclerosis. Target irisan kemudian dianalisis menggunakan STRING untuk membangun jaringan Protein–Protein Interaction (PPI) dengan confidence ≥ 0,400, kemudian divisualisasikan dan dianalisis topologinya di Cytoscape guna mengidentifikasi protein sentral. 

[Screenshot_20260806_160831.jpg](/Screenshot_20260806_160831.jpg "Screenshot_20260806_160831")
Gambar 1. Irisan gen target  atherosclerosis dan Senyawa target 

Berdasarkan hasil analisis, diperoleh 188 gen yang berasosiasi dengan atherosclerosis dan 337 protein target hasil prediksi dari keenam senyawa menggunakan SwissTargetPrediction. Irisan kedua kelompok tersebut menghasilkan 14 gen target potensial yang diperkirakan berperan sebagai mediator utama efek farmakologis senyawa terhadap penyakit. Daftar gen irisan tersebut dimasukkan ke dalam platform STRING untuk konstruksi jaringan dan identifikasi hub protein dengan mencari top 9 target utama menggunakan cytoHubba. 

Tabel 1. Nilai degree, betweenness centrality, dan closeness centrality dari 9 hub gen teratas hasil analisis jaringan PPI


Analisis topologi jaringan PPI menunjukkan bahwa PPARG merupakan hub protein utama dengan nilai degree (6), betweenness centrality (0,6786), dan closeness centrality (0,8000) tertinggi dibandingkan protein lainnya. Temuan ini menegaskan bahwa PPARG berperan sebagai penghubung utama antarprotein dalam jaringan, sehingga menjadi titik fokus dalam mekanisme molekuler. Selain PPARG, protein lain seperti NR1H3, FABP4, MMP3, dan PPARD juga menunjukkan konektivitas tinggi yang mengindikasikan keterlibatan dalam homeostasis lipid, stabilitas plak, dan inflamasi vaskular. 
Gambar 2. Jaringan Protein-Protein Interaction (PPI) dari 14 gen irisan hasil konstruksi STRING
Analisis Protein–Protein Interaction (PPI) menunjukkan bahwa ke-14 gen irisan membentuk jaringan interaksi yang saling terhubung, mengindikasikan adanya hubungan fungsional dalam patogenesis aterosklerosis. Berdasarkan visualisasi jaringan, PPARG berada pada posisi sentral dengan jumlah koneksi terbanyak terhadap protein lain, seperti NR1H3, PPARD, FABP4, ESR1, MMP3, dan ALOX5. Posisi tersebut menunjukkan bahwa PPARG berpotensi menjadi regulator utama dalam mengendalikan metabolisme lipid, respons inflamasi, dan homeostasis kolesterol. Selain itu, interaksi erat antara PPARG dan NR1H3 mengindikasikan keterlibatan jalur regulasi lipid yang berperan penting dalam mencegah pembentukan foam cell dan progresi plak aterosklerosis. Dengan demikian, protein-protein yang berada pada pusat jaringan diperkirakan menjadi target molekuler utama dari senyawa bioaktif yang dianalisis 


 
Gambar 3. Visualisasi jaringan interaksi senyawa–target–pathway
Visualisasi compound–target–pathway network menunjukkan hubungan antara lima senyawa aktif dengan protein target serta PPAR signaling pathway sebagai jalur biologis utama hasil enrichment analysis. Integrasi ini memperlihatkan bagaimana setiap senyawa mampu berinteraksi dengan lebih dari satu protein target, sehingga efek farmakologisnya terjadi secara sinergis. Di antara protein tersebut, PPARG tampak memiliki konektivitas tertinggi karena menjadi titik temu beberapa senyawa sekaligus terhubung dengan jalur PPAR signaling pathway. 





 Gambar 4. Hasil enrichment analysis Gene Ontology (Biological Process, Molecular Function) dan KEGG Pathway terhadap target irisan

Hasil enrichment analysis menunjukkan bahwa protein target memiliki keterlibatan signifikan dalam berbagai fungsi molekuler, proses biologis, dan jalur pensinyalan yang berkaitan dengan patogenesis aterosklerosis. Pada kategori Gene Ontology (Molecular Function), fungsi yang paling dominan meliputi long-chain fatty acid binding, lipid binding, dan nuclear receptor activity, yang mengindikasikan peran protein target dalam regulasi metabolisme lipid dan homeostasis kolesterol. Sementara itu, Gene Ontology (Biological Process) menunjukkan keterlibatan protein target dalam regulasi respons inflamasi, regulasi pertahanan tubuh, penyimpanan kolesterol, dan metabolisme asam lemak, yang merupakan proses penting dalam pembentukan plak aterosklerosis. Selain itu, analisis KEGG Pathway mengidentifikasi PPAR signaling pathway sebagai jalur biologis utama yang berperan dalam mengatur metabolisme lipid, menghambat pembentukan foam cell, dan menekan inflamasi vaskular. Hasil ini menunjukkan bahwa senyawa bioaktif diperkirakan bekerja melalui modulasi PPAR signaling pathway sehingga berpotensi memperlambat progresi aterosklerosis melalui mekanisme multi-target 


## Referensi
Ji, L., Song, T., Ge, C., Wu, Q., Ma, L., Chen, X., Chen, T., Chen, Q., Chen, Z., & Chen, W. (2023). Identification of bioactive compounds and potential mechanisms of scutellariae radix-coptidis rhizoma in the treatment of atherosclerosis by integrating network pharmacology and experimental validation. Biomedicine & pharmacotherapy = Biomedecine & pharmacotherapie, 165, 115210. https://doi.org/10.1016/j.biopha.2023.115210   
Xie, X., Ma, X., Zeng, S., Tang, W., Xiao, L., Zhu, C., & Yu, R. (2020). Mechanisms of Berberine for the Treatment of Atherosclerosis Based on Network Pharmacology. Evidence-based complementary and alternative medicine : eCAM, 2020, 3568756. https://doi.org/10.1155/2020/3568756 
