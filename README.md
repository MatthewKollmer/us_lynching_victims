# The Victim-Centered Dataset of U.S. Lynching Newspaper Reports

<p align="center">
  <img src="https://github.com/MatthewKollmer/us_lynching_victims/blob/162d745fafe7398c7627f6b887f976084d426459/figure_4_lynch_locations.png" width="700" height="450">
</p>
</div>
<p align="center">Map of US Lynching Locations in the Victim-Centered Dataset</p>

The US Lynching Victims Project is one sub-project in the larger [Virality of Racial Terror Project (VRT)](https://www.racialviolencearchive.com/vrt-project.html), a grant-funded initiative that applies computational methods to identify and study the circulation of racial violence reports in the United States between 1865 and 1921. In that regard, the US Lynching Victims Project specifically relies on existing datasets of lynchings from the period. It builds off a century's worth of work by journalists, activists, and researchers–from Ida B. Wells-Barnett, Monroe Work, the NAACP, and many others–who collectively documented instances of lynchings and racial violence over many decades. Thanks to this rich tradition of activism through research, we have data that provides victim names, places, and dates, and in turn, a much better understanding of the appalling legacy of racial violence in the United States.

Two resources, more recently compiled, have become integral to the US Lynching Victims Project. They are the [Seguin-Rigby Dataset](https://journals.sagepub.com/doi/full/10.1177/2378023119841780) and the [Tolnay-Beck Inventory](https://www.press.uillinois.edu/books/?id=p064135). Together they include documentation of thousands of victims of racial violence. Both resources were compiled by sociologists and researchers who investigated numerous other sources and archives. Using their data, the US Lynching Victims Project has built a pipeline for text-mining digitized newspapers in order to identify reports and reprintings of lynchings. The results of our work include newly curated data composed of lynching reports from the era. This data allows us to study racial violence reporting at numerous scales–from individual cases of racial violence, to regional, local, and national responses to the broader phenomenon of lynching.

This repository is a presentation of code from the US Lynching Victims Project. It is intended to make our pipeline more easily replicable and reviewed. Please note that this work is ongoing, and so this repository will see many updates in the near future. But if you'd like to follow along, you can retrace every computational step in the following Python notebooks:

1) unify our data sources (see [01_unify_data_sources.ipynb](https://github.com/MatthewKollmer/us_lynching_victims/blob/main/01_unify_data_sources.ipynb))
2) pull search results from Chron Am (see [02_pull_search_results.ipynb](https://github.com/MatthewKollmer/us_lynching_victims/blob/main/02_pull_search_results.ipynb))
3) scrape search results (see [03_scrape_search_results.ipynb](https://github.com/MatthewKollmer/us_lynching_victims/blob/main/03_scrape_search_results.ipynb))
4) enrich our datasets (see [04_enrich_dataset.ipynb](https://github.com/MatthewKollmer/us_lynching_victims/blob/main/04_enrich_dataset.ipynb))
5) select a random sample (see [05_random_sample.ipynb](https://github.com/MatthewKollmer/us_lynching_victims/blob/main/05_random_sample.ipynb))
6) label the training data (see [06_label_training_data.ipynb](https://github.com/MatthewKollmer/us_lynching_victims/blob/main/06_label_training_data.ipynb))
7) fine-tune BERT and classify data (see [07_BERT_classifier.ipynb](https://github.com/MatthewKollmer/us_lynching_victims/blob/main/07_BERT_classifier.ipynb))
8) enrich our data with locations (see [08_enrich_dataset_x2.ipynb](https://github.com/MatthewKollmer/us_lynching_victims/blob/main/08_enrich_dataset_x2.ipynb))
9) interactive codebook (see [09_interactive_codebook.ipynb](https://github.com/MatthewKollmer/us_lynching_victims/blob/main/09_interactive_codebook.ipynb) or visit [https://matthewkollmer.com/09_interactive_codebook.html](https://matthewkollmer.com/09_interactive_codebook.html) to interact with the codebook directly))

To understand the genesis of this project, you may also want to review my draft version here: [https://github.com/MatthewKollmer/works-in-progress/tree/main/vrt_work/us-lynching-victims](https://github.com/MatthewKollmer/works-in-progress/tree/main/vrt_work/us-lynching-victims). This draft version shows how the project involved numerous iterations, failed attempts, explorations, and non-linear processes. It contains journal entries alongside code and other resources. The draft version is admittedly more convoluted, but it's also a fully transparent resource that highlights the many _processes_ involved in this kind of work.

If you need access to the data, please [contact me](https://matthewkollmer.com/contact/). Once I send you an invite, the US Lynching Victims data can be found here: [https://uofi.app.box.com/folder/311999767132](https://uofi.app.box.com/folder/311999767132)
