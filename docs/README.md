# Biomarker Discovery: from theory to real world examples

Welcome to the workshop
'Biomarker Discovery: from theory to real world examples'

- [Prerequisites](prerequisites.md)
- [FAQ](faq.md)
- [Contact us](contact_us.md)

```mermaid
flowchart TD
    biomarker_discovery
    study_design
    internal_and_external_validation
    big_tabular_data
    many_more_traits_than_samples
    look_for_correlations
    care_about_predictive_power
    do_not_look_for_causation
    risk_of_overfitting
    do_not_care_about_causation
    performance_indicators
    
    biomarker_discovery --> |uses| big_tabular_data
    biomarker_discovery --> |has| study_design

    big_tabular_data --> look_for_correlations
    big_tabular_data --> care_about_predictive_power

    big_tabular_data --> |has| many_more_traits_than_samples
    many_more_traits_than_samples --> |causes| risk_of_overfitting
    risk_of_overfitting <--> internal_and_external_validation
    many_more_traits_than_samples --> |needs| internal_and_external_validation

    look_for_correlations --- do_not_look_for_causation
    care_about_predictive_power --- do_not_care_about_causation
    care_about_predictive_power --- performance_indicators
    
    
    study_design --> |helps establish| internal_and_external_validation
```

## Old stuff

- [Communication](communication.md)

