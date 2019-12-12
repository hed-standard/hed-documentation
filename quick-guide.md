Most people who worked with EEG data are familiar with the practice of using lab-specific labels or arbitrary integers to annotate what and when events happened during an experiment. Re-using a collected dataset for new analysis means reading carefully the experiment description to understand the meaning of those event codes. Meanwhile, the success of data sharing efforts have now allowed EEG researchers to access an increasing number of dataset from many studies, which also made this manual reading process ever more debilitating. Moreover, the lack of details expressed in an event code prevents researchers from flexibly combine events across studies using the nature of experimental events, nor able to be effeciently evaluate which events to be included in their analysis. These constraints make the exploration of applying recent advances in machine learning for large-scale EEG analysis infeasible.

Hierarchical Event Descriptor (HED) provides a standardized way to describe precisly the nature of the experimental events. With HED-annotated datasets, researchers will easily undertand the meaning of event codes without even reading the experiment description. Moreover, analysis tools will be able to aggregate events across a large number of studies with minimal human supervision. The HED system comprises of a schema and the software ecosystem supporting the annotation, validation, and extraction of EEG events using HED tags. The [HED schema](http://www.hedtags.org/display_hed.html) specifies the collection of HED tags to annotate events, organized in a hierarchical structure. HED-supporting software currently includes the EEGLAB plug-in [HEDTools](https://github.com/hed-standard/hed-matlab/tree/master/EEGLABPlugin), the tagging program [CTAGGER](https://github.com/hed-standard/hed-java/blob/master/java/tagging/CTagger.jar) (which is also bundled with the EEGLAB plug-in HEDTools), and online [HED validator](http://visual.cs.utsa.edu/hed/validation).

This guide will focus on the EEGLAB plug-in *HEDTools* for event annotation, extraction, and validation using HED tags. After this guide, you will be familiarized with the HED schema and how to associate HED tags with your events. You will also see how you can use HED-annotated events for your analysis. These knowledge will transfer beyond the EEGLAB environment, and you can use other tool system to work with HED.



[I. Event annotation & extraction with EEGLAB plug-in *HEDTools*](#I)

1. [What is EEGLAB?](#I.1)
2. [Installing EEGLAB and load dataset](#I.2)
3. [Adding tags using CTAGGER](#I.3)
4. [Validating tagged dataset](#I.4)
5. [Extracting HED-annotated events](#I.5)

[II. HED schema and the art of tagging](#II)



## <a name="I">I. Event annotation & extraction with EEGLAB plug-in *HEDTools*</a>
#### <a name="I.1">1. What is EEGLAB?</a>

[EEGLAB](https://sccn.ucsd.edu/eeglab/index.php) is one of the world most widely used EEG analysis toolbox. It combines both graphical and command-line user interface, which is friendly for both beginner and those who prefer a more flexible, automated way of analyzing data. This quick guide will show how you can work with HED in EEGLAB using both interfaces. If you are familiar with EEGLAB, you can skip the next section on EEGLAB installation and jump to [section I.3](#I.3) to start learning how to tag your loaded data with HED.

#### <a name="I.2">2. Installing EEGLAB and load dataset</a>


#### <a name="I.3">3. Adding tags using CTAGGER</a>

#### <a name="I.4">4. Validating tagged dataset</a>

#### <a name="I.5">5. Extracting HED-annotated events</a>



## <a name="II">II. HED schema and the art of tagging</a>


