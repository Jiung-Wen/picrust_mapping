# MetaCyc mapfiles for PICRUSt2

These mapfiles are created for PICRUSt2's [add_description](https://github.com/picrust/picrust2/wiki/Add-descriptions) script to group MetaCyc pathways into few categories.
```
add_descriptions.py -i pathways_out/path_abun_unstrat.tsv
                    --custom_map_tabl ../metacyc_pathways_info_prokaryotes_top_level.tsv
                    -o pathways_out/path_abun_unstrat_descrip.tsv
```

The ```top level``` of MetaCyc pathway looks like [this](https://metacyc.org/META/class-tree?object=Pathways), while the ```second level``` is the child classes of the top classes.

Though this level may not be analogous to KEGG's BRITE hierarchy, it gives me a quick insight of the predictedd pathways.

Please note that some pathways belong to more than one class. For example, pathway [PWY-7013](https://metacyc.org/META/NEW-IMAGE?type=PATHWAY&object=PWY-7013) belongs to both **Degradation/Utilization/Assimilation** and **Generation of Precursor Metabolite and Energy** classes. However, I was not aware of this by the time I create the mapfiles. So always check the MetaCyc website if you have any question.

Also note that I accessed the MetaCyc website to create these mapfiles at Dec. 2, 2018, so the pathway description is subject to change.
