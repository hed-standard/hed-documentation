**Events should have HED tags**: ("What does '*Event code 17*' mean?") Traditionally, software systems for event-related EEG data collection and analysis have used simple numeric codes (2,17, 253) whose meaning is hopefully saved with the data somewhere, or else given a brief text label ('*Target*'). But with the creation and availability of new analysis methods for extracting information, EEG data are valuable long after their first publication, and will in near future become even more so as public *data archives and tool repositories (DATRs)* become active and available. Archiving data in private or public DATRs allows further, intensive data analyses as well as meta-analyses across studies with different designs. All of this requires that the more exact nature of the recorded experimental events are saved and accessible in an agreed format. Today the *only* such format is the **Hierarchical Event Descriptor (HED)** system of Nima Bigdely-Shamlo, Kay Robbins developed at the Swartz Center, UCSD (REF). Accordingly, HED has been accepted in the rapidly emerging BIDS standards for data archive. In conjunction with a project to build a DATR ('NEMAR') for human neuroelectromagnetic data under NIMH funding, we (Scott Makeig, Arno Delorme, Amit Majumdar, Russ Poldrack) and our colleagues are creating and polishing tools to make adding more detailed HED tag descriptions of experimental events to new or existing data as simple as possible, and for using HED tags within EEGLAB to create custom event collections based on their detailed HED tag descriptions. Enhanced HED tutorial websites and videos we will be online soon.

**HED Tagging**: Most people who have worked with EEG data are familiar with the practice of using brief lab-specific labels (*'Target'*) or arbitrary integers (*'event type 17'*) to annotate what events happened when during an experiment. Re-using a collected dataset for new analysis then involves reading the reported experiment description carefully (if available) to gain some meaning of those event codes. However, the lack of detail expressed in an event code prevents researchers from flexibly combining events across studies based on the precise nature of experimental events (*'Are green stimuli processed differently than red, no matter their shape?'*, *'Is there any EEG biomarker of the participant having viewed a bridsound rather than a sine tone?'*, etc.). Nor are researchers able to most efficiently evaluate which events to include in their analysis (*'Only blue targets??'*). Meanwhile, the success of various data sharing efforts now begin to allow EEG researchers to access an increasing number of datasets from many studies involving different designs. This opens the possibility of applying advanced machine learning algorithms to analyze EEG dynamics based on a larger and more diverse scale of data. Unfortunately, it would be infeasible to actualize these possibilities, given the constraints imposed by current practises in experimental event annotation.

**The HED System**:The *Hierarchical Event Descriptor (HED)* system provides a standardized way to describe precisely the nature of recorded or later identified experimental events. Using HED-tagged datasets, researchers will no longer have to deal with meaningless event codes. Moreover, analysis tools will be able to aggregate events across a large number of studies with minimal human supervision. The HED system comprises a schema (syntax and agreed upon top-level tag hierarchy) and a software ecosystem supporting annotation, validation, and extraction of EEG events using HED tags. The [*HED schema*](http://www.hedtags.org/display_hed.html) specifies a collection of HED tags in use to annotate events, organized in a partially hierarchical structure. Software supporting the use of HED event tagging currently includes the EEGLAB plug-in [*HEDTools*](https://github.com/hed-standard/hed-matlab/tree/master/EEGLABPlugin), the GUI-based tagging program [*CTAGGER*](https://github.com/hed-standard/hed-java/blob/master/java/tagging/CTagger.jar) (now bundled with the *HEDTools* plug-in), and the online [*HED validator*](http://visual.cs.utsa.edu/hed/validation).

**HEDTools**: This guide will focus on the EEGLAB plug-in *HEDTools* for event annotation, extraction, and validation using HED tags. After reading this guide, you will be familiar with the HED schema and how to associate HED tags with events. You will also see how you can use HED-annotated events in your analysis. Your understanding will generalize beyond the EEGLAB environment, as you can use any other data analysis tool environment to work with HED.


[I. Event annotation & extraction with EEGLAB plug-in *HEDTools*](#I)

1. [What is EEGLAB?](#I.1)
2. [Installing EEGLAB and load dataset](#I.2)
3. [Adding tags using CTAGGER](#I.3)
4. [Validating tagged dataset](#I.4)
5. [Extracting HED-annotated events](#I.5)

[II. HED schema and the art of tagging](#II)



## <a name="I">I. Event annotation & extraction with EEGLAB plug-in *HEDTools*</a>
#### <a name="I.1">1. What is EEGLAB?</a>

[EEGLAB](https://sccn.ucsd.edu/eeglab/index.php) is a most widely used EEG software environment for analysis of human electrophsyioloigcal (and related) data. It combines both graphical and command-line user interfaces, making it friendly for both beginners who may who prefer a more flexible, automated way of analyzing data, and experts, who can easily extend the EEGLAB tool environment by making new EEGLAB compatible functions and/or publishing EEGLAB plug-in toolboxes that are then immediately available, through the EEGLAB graphic user interface (GUI) to anyone who downloads them. This quick guide will show how you can work with HED in EEGLAB. If you are familiar with EEGLAB, you can skip the next section on EEGLAB installation and jump to [section I.3](#I.3) to learn how to tag data using HED.

#### <a name="I.2">2. Installing EEGLAB and loading datasets in EEGLAB</a>


#### <a name="I.3">3. Adding tags using CTAGGER</a>

#### <a name="I.4">4. Validating a HED-tagged dataset</a>

#### <a name="I.5">5. Extracting HED-tagged events and event-locked data epochs from an EEGLAB dataset</a>

## <a name="II">II. The HED schema and the art of event annotation</a>


