# MBED Today

A phone-first view of Mary Bridge Emergency Department's day, for staff.

**https://ted72782.github.io/mbed-today/**

Three tabs:

| tab | staff enter | it shows |
|---|---|---|
| **Arrivals** | patients registered since midnight | today's projected total, with a likely range |
| **Evening wait** | waiting-room count and total in department | tonight's worst-stretch wait for a room |
| **Today's risk** | arrivals so far | whether today is tracking toward a bad day |

## What is published here

Aggregate, department-level numbers only — hourly and daily counts, average waiting
times, and the fitted models behind each tab. **No patient-level data, no identifiers
and no staff names are published.** Every file here is derived from a de-identified
database and contains counts and averages.

## How it updates

The pages and their data files are rebuilt automatically from the MBED pipeline and
pushed here when they change. This repository holds published output only; the models,
the guards and the source live in the private MBED repository.

## Honest limits, stated on the pages themselves

Each tab reports the hours it is reliable from, measured out of sample, and goes quiet
when it is not:

- **Arrivals** is not reliable before 09:00.
- **Evening wait** is not reliable before 18:00.
- **Today's risk** has no skill below about 125 arrivals a day and says so rather than
  showing a number.

These tools indicate how a day is tracking. They do not establish what will fix it.
