# Learning the Beauty in Songs: Neural Singing Voice Beautifier

Jinglin Liu, Chengxi Li, Yi Ren, Zhiying Zhu, Zhou Zhao

Zhejiang University

ACL 2022 Main conference

Code project: [NeuralSVB](https://github.com/MoonInTheRiver/NeuralSVB) [![](https://img.shields.io/github/stars/MoonInTheRiver/NeuralSVB)](https://github.com/MoonInTheRiver/NeuralSVB)


Related project: [DiffSinger](https://github.com/MoonInTheRiver/DiffSinger) [![](https://img.shields.io/github/stars/MoonInTheRiver/DiffSinger)](https://github.com/MoonInTheRiver/DiffSinger) [![downloads](https://img.shields.io/github/downloads/MoonInTheRiver/DiffSinger/total.svg)](https://github.com/MoonInTheRiver/DiffSinger/releases)

## Abstract

We are interested in a novel task, singing voice beautifying (SVB). Given the singing voice of an amateur singer, SVB aims to improve the intonation and vocal tone of the voice, while keeping the content and vocal timbre. Current automatic pitch correction techniques are immature, and most of them are restricted to intonation but ignore the overall aesthetic quality. Hence, we introduce Neural Singing Voice Beautifier (NSVB), the first generative model to solve the SVB task, which adopts a conditional variational autoencoder as the backbone and learns the latent representations of vocal tone. In NSVB, we propose a novel time-warping approach for pitch correction: Shape-Aware Dynamic Time Warping (SADTW), which ameliorates the robustness of existing time-warping approaches, to synchronize the amateur recording with the template pitch curve. Furthermore, we propose a latent-mapping algorithm in the latent space to convert the amateur vocal tone to the professional one. Extensive experiments on both Chinese and English songs demonstrate the effectiveness of our methods in terms of both objective and subjective metrics. 

<img align="center" src="resources/model_all7.png" style="  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 100%;" />
<img align="center" src="resources/melhhh2.png" style="  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 100%;" />

## Singing Audio Samples
Note that the singer in the testing data could **not** be found in the training data.
### Chinese
0. ???????????????????????????, sh?? ji?? b?? n?? xi??ng xi??ng zh??ng m??ng l??ng
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_p/19.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_a/19.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/baseline/19.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/NSVB/19.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>
1. ???????????????, b?? hu?? y?? ch??ng k??ng
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_p/18.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_a/18.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/baseline/18.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/NSVB/18.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>
2. ???????????????????????????, b?? sh?? ti??n q??ng ji?? hu?? y??u c??i h??ng
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_p/21.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_a/21.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/baseline/21.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/NSVB/21.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>

3. ??????????????????, y??o r?? h?? z??i s??u su??
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_p/1.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_a/1.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/baseline/1.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/NSVB/1.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>

4. ?????????????????????????????????, y?? x?? w??i l??i y??o yu??n z??i gu??ng ni??n zh?? w??i
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_p/2.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_a/2.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/baseline/2.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/NSVB/2.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>

5. ????????????????????????, z?? g??u d?? d??ng ti??n xu??n d?? zhu??n
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_p/3.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_a/3.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/baseline/3.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/NSVB/3.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>

6. ??????????????????, su?? r??n y?? sh?? hu?? hu??
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_p/4.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_a/4.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/baseline/4.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/NSVB/4.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>

7. ?????????????????????, c??ng l??i y?? b?? ju?? d?? cu??
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_p/5.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_a/5.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/baseline/5.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/NSVB/5.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>
<!-- 9. ?????????????????????, xi??o w?? g??i b?? q?? ch??ng nu??
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_p/14.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_a/14.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/baseline/14.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/NSVB/14.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table> -->
### English
0. I'm not angry anymore
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/English/gt_p/21.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/gt_a/21.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/baseline/21.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/NSVB/21.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>
1. and the band won't play
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/English/gt_p/1.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/gt_a/1.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/baseline/1.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/NSVB/1.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>
2. it's love
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/English/gt_p/20.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/gt_a/20.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/baseline/20.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/NSVB/20.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>
3. the days grow long
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/English/gt_p/2.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/gt_a/2.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/baseline/2.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/NSVB/2.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>

4. were beautiful like diamonds in the sky
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/English/gt_p/7.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/gt_a/7.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/baseline/7.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/NSVB/7.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>

5. cause I wanna be better than I was before
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/English/gt_p/14.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/gt_a/14.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/baseline/14.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/NSVB/14.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>

6. I'll fix you with my love
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/English/gt_p/13.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/gt_a/13.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/baseline/13.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/NSVB/13.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>
7. we will glow in the dark turning dust to gold
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/English/gt_p/9.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/gt_a/9.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/baseline/9.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/English/NSVB/9.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>
### Special cases on dialect
1. ???????????????, ????????? gua sin khia peh be, tsau sam kuan
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_p/16.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_a/16.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/baseline/16.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/NSVB/16.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>

2. ??????????????????,????????? gua kai uann soo i, hue tiong guan
    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT Professional</th>
            <th>GT Amateur</th>
            <th>baseline</th>
            <th>NSVB</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_p/17.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/gt_a/17.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/baseline/17.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/Chinese/NSVB/17.wav" type="audio/wav"></audio></td>
        </tr>
    </tbody>
    </table>
