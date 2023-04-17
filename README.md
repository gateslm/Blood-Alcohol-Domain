# Blood-Alcohol-Domain
Blood Alcohol Domain with additional files about processing and background information. 

We were provided permission by the authors of the data set to make it publicly accessible. 

## Referencing the Dataset

When utilizing this dataset, please cite this paper and include the repository URL in a footnote for future researchers to find as well. 

```tex
TODO
```

The footnote you should include for reaching the dataset:

```tex
\footnote{GitHub Link: \url{https://github.com/gateslm/Blood-Alcohol-Domain}}
```

## Files Included

The following files are included: 
1. `detailed_data.csv`
2. `README.md` (This file)

The `csv` file has a header to detail which column is which feature. 

## About the Dataset

```tex
@phdthesis{doyle05,
  title={A knowledge-light mechanism for explanation in case-based reasoning},
  author={Doyle, D{\'o}nal},
  year={2005},
  school={University of Dublin, Trinity College. Department of Computer Science},
  note={Thesis at \url{http://www.tara.tcd.ie/handle/2262/847}.}
}
```

The dataset is from the D. Doyle Thesis (BibTex above). The additional information we found about the dataset is at the following links:
- [Abstract of Project](https://web.archive.org/web/20010826182630/http://www.cs.tcd.ie/~doylemi/abstract.html)
- [Feature Description](https://web.archive.org/web/20010722131007fw_/http://www.maths.tcd.ie/~mdoyle/java/javahtml/form.html)
- [Blood Alcohol Content Table](https://web.archive.org/web/20010722131337fw_/http://www.maths.tcd.ie/~mdoyle/java/javahtml/table.html)

The original dataset was in XML format. All features were preserved in the conversion from XML to CSV. 

## Features

### Gender
Options are `male` and `female`. 

### Frame Size
There are 8 possible values from 1 to 8, correspoinding to weight ranges (100-119, ..., 240+). 

### Amount Consumed
Ranges between 1 to 14 drinks (inclusive). It is the amount of drinks consumed. 

### Meal
The meal attribute refers to the amount an indiviaul ate while drinking: full meal, snack, and none. 

### Duration
Duration is the amount of time the person drank alcohol. Duration was either 30, 60, 90, 120, 150, 180, 210 or 240 minutes. 

### BAC
Initial BAC values ranged from 0.1 to 1.0+ inclusive, we converted these to a binary over or under the limit, which was presented to the participants.  Following the link above (Blood Alcohol Content Table), the data can be converted to `over` and `under`. 