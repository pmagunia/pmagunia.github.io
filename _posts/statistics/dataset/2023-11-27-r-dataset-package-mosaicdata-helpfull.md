---
title: R Dataset / Package mosaicData / HELPfull
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">HELPfull</span> data set which pertains to Health Evaluation and Linkage to Primary Care. The <span class="mono">HELPfull</span> data set is found in the <span class="mono">mosaicData</span> R package. You can load the <span class="mono">HELPfull</span> data set in R by issuing the following command at the console <span class="mono">data("HELPfull")</span>. This will load the data into a variable called <span class="mono">HELPfull</span>. If R says the <span class="mono">HELPfull</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("mosaicData")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-90830.csv">HELPfull R data set</a></span>. The size of this file is about 2,915,134 bytes.</p><h2>Health Evaluation and Linkage to Primary Care</h2>
<h3>Description</h3>
<p>The HELP study was a clinical trial for adult inpatients recruited from a detoxification unit. Patients with no primary care physician were randomized to receive a multidisciplinary assessment and a brief motivational intervention or usual care, with the goal of linking them to primary medical care.</p>
<h3>Usage</h3>
<pre>
data(HELPfull)
</pre>
<h3>Format</h3>
<p>A data frame with 1472 observations on the following variables.</p>
<ul>
<li>
<p><code>ID</code> Subject ID</p>
</li>
<li>
<p><code>TIME</code> Interview time point</p>
</li>
<li>
<p><code>NUM_INTERVALS</code> Number of 6-month intervals from previous to current interview</p>
</li>
<li>
<p><code>INT_TIME1</code> # of months from baseline to current interview</p>
</li>
<li>
<p><code>DAYS_SINCE_BL</code> # of days from baseline to current interview</p>
</li>
<li>
<p><code>INT_TIME2</code> # of months from previous to current interview</p>
</li>
<li>
<p><code>DAYS_SINCE_PREV</code> # of days from previous to current interview</p>
</li>
<li>
<p><code>PREV_TIME</code> Previous interview time</p>
</li>
<li>
<p><code>DEAD</code> a numeric vector</p>
</li>
<li>
<p><code>A1</code> Gender (1=Male, 2=Female)</p>
</li>
<li>
<p><code>A9</code> Years of education completed</p>
</li>
<li>
<p><code>A10</code> Marital Status (1=Married, 2=Remarried, 3=Widowed, 4= Separated, 5=Divorced, 6=Never Married</p>
</li>
<li>
<p><code>A11A</code> Do you currently have a living mother? (0=No, 1= Yes</p>
</li>
<li>
<p><code>A11B</code> Do you currently have a living father? (0=No, 1=Yes</p>
</li>
<li>
<p><code>A11C</code> Do you currently have siblings? (0=No, 1=Yes</p>
</li>
<li>
<p><code>A11D</code> Do you currently have a partner (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A11E</code> Do you currently have children? (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A12B</code> Hollingshead categories (1=Major profess, 2= Lesser profess, 3=Minor profess, 4=Clerical/sales, 5=Skilled manual, 6=Semi-skilled, 7=Unskilled, 8= Homemaker, 9=No occupation)</p>
</li>
<li>
<p><code>A13</code> Usual employment pattern in last 6 months (1=Full time, 2= Part time, 3=Student, 4=Unemployed, 5=Control envir)</p>
</li>
<li>
<p><code>A14A</code> Loved alone-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A14B</code> Lived w/a partner-last 6 mos (0=No, 1=Yes</p>
</li>
<li>
<p><code>A14C</code> Lived with parent(s)-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A14D</code> Lived w/children-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A14E</code> Lived w/other family-last 6 mos (0=No, 1=Yes</p>
</li>
<li>
<p><code>A14F</code> Lived w/friend(s)-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A14G</code> Lived w/other-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A14G_T</code> a factor with levels <code>1/2 WAY HOUSE</code> <code>3/4 HOUSE</code> <code>ANCHOR INN</code> <code>ARMY</code> <code>ASSOCIATES</code> <code>BOARDERS</code> <code>BOYFRIENDS MOM</code> <code>CORRECTIONAL FACILIT</code> <code>CRACK HOUSE</code> <code>DEALER</code> <code>ENTRE FAMILIA</code> <code>FENWOOD</code> <code>GAVIN HSE</code> <code>GIRLFRIENDS DAUGHTE</code> <code>GIRLFRIENDS SON</code> <code>GIRLFRIENDS CHILDREN</code> <code>GIRLFRIENDS DAUGHTER</code> <code>GROUP HOME</code> <code>HALF-WAY HOUSE</code> <code>HALFWAY HOUSE</code> <code>HALFWAY HOUSES</code> <code>HALFWAY HSE</code> <code>HOLDING UNIT</code> <code>HOME BORDER</code> <code>HOMELESS</code> <code>HOMELESS SHELTER</code> <code>IN JAIL</code> <code>IN PROGRAMS</code> <code>INCARCERATED</code> <code>JAIL</code> <code>JAIL HALFWAY HOUSE</code> <code>JAIL, SHELTER</code> <code>JAIL, STREET</code> <code>JAIL/PROGRAM</code> <code>JAIL/SHELTER</code> <code>JAILS</code> <code>LANDLADY</code> <code>LANDLORD</code> <code>LODGING HOUSE</code> <code>MERIDIAN HOUSE</code> <code>NURSING HOME</code> <code>ON THE STREET</code> <code>PARTNERS MOTHER</code> <code>PARTNERS CHILD</code> <code>PARTNERS CHILDREN</code> <code>PRDGRAMS</code> <code>PRISON</code> <code>PROGRAM</code> <code>PROGRAM MTHP</code> <code>PROGRAM ROOMMATES</code> <code>PROGRAM SOBER HOUSE</code> <code>PROGRAM-RESIDENTIAL</code> <code>PROGRAM/HALFWAY HOUS</code> <code>PROGRAM/JAIL</code> <code>PROGRAM/SHELTER</code> <code>PROGRAM/SHELTERS</code> <code>PROGRAMS</code> <code>PROGRAMS SUBSTANCE</code> <code>PROGRAMS/SHELTER</code> <code>PROGRAMS/SHELTERS</code> <code>PROGRAMS/SHELTERS/DE</code> <code>PROJECT SOAR</code> <code>RESIDENTIAL FACILITY</code> <code>RESIDENTIAL PROGRAM</code> <code>ROOMING HOUSE</code> <code>ROOMING HOUSE (RELIG</code> <code>ROOMMATE</code> <code>ROOMMATES</code> <code>ROOMMATES AT TRANSIT</code> <code>RYAN HOUSE</code> <code>SALVATION ARMY</code> <code>SHELTER</code> <code>SHELTER/HALFWAY HSE</code> <code>SHELTER/HOTEL</code> <code>SHELTER/PROGRAM</code> <code>SHELTERS</code> <code>SHELTERS/HOSPITALS</code> <code>SHELTERS/JAIL</code> <code>SHELTERS/PROGRAMS</code> <code>SHELTERS/STREETS</code> <code>SOBER HOUSE</code> <code>SOBER HOUSING</code> <code>SOUTH BAY JAIL</code> <code>STEPSON</code> <code>STREET</code> <code>STREETS</code> <code>SUBSTANCE ABUSE TREA</code> <code>TRANSITIONAL HOUSE</code> <code>VA SHELTER</code></p>
</li>
<li>
<p><code>A15A</code> #nights in ovrnight shelter-last 6 mos</p>
</li>
<li>
<p><code>A15B</code> # nights on street-last 6 mos</p>
</li>
<li>
<p><code>A15C</code> #months in jail-last 6 mos</p>
</li>
<li>
<p><code>A16A</code> # months in ovrnight shelter-last 5 yrs</p>
</li>
<li>
<p><code>A16B</code> #moths on street-last 5 yrs</p>
</li>
<li>
<p><code>A16C</code> #months in jail-last 5 yrs</p>
</li>
<li>
<p><code>A17A</code> Received SSI-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A17B</code> Received SSDI-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A17C</code> Received AFDC-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A17D</code> Received EAEDC-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A17E</code> Received WIC-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A17F</code> Received unemployment benefits-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A17G</code> Received Workman's Comp-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A17H</code> Received Child Support-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A17I</code> Received other income-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A17I_T</code> a factor with levels <code>DISABLED VETERAN</code> <code>EBT (FOOD STAMPS)</code> <code>EMERGENCY FOOD STAMP</code> <code>FOOD STAMP</code> <code>FOOD STAMPS</code> <code>FOOD STAMPS/VETERAN</code> <code>FOOD STAMPS/VETERANS</code> <code>INSURANCE SETTLEMENT</code> <code>PENSION CHECK</code> <code>SECTION 8</code> <code>SERVICE CONNECTED DI</code> <code>SOCIAL SECURITY</code> <code>SSDI FOR SON</code> <code>SURVIVORS BENEFITS</code> <code>TEMPORARY DISABILITY</code> <code>VA BENEFITS-DISABILI</code> <code>VA COMPENSATION</code> <code>VA DISABILITY PENSIO</code> <code>VETERAN BENEFITS</code> <code>VETERANS SERVICES</code> <code>VETERANS AFFAIRS</code></p>
</li>
<li>
<p><code>A18</code> Most money made in any 1 year-last 5 yrs (1=&lt;5000, 2=5000-10000, 3=11000-19000, 4=20000-29000, 5=30000-39000, 6=40000-49000, 7=50000+</p>
</li>
<li>
<p><code>B1</code> In general, how is your health (1=Excellent, 2=Very Good, 3=Good, 4=Fair, 5=Poor)</p>
</li>
<li>
<p><code>B2</code> Comp to 1 yr ago, how is your health now (1=Much better, 2=Somewhat better, 3=About the same, 4=Somewhat worse, 5=Much worse)</p>
</li>
<li>
<p><code>B3A</code> Does health limit you in vigorous activity (1=Limited a lot, 2=Limited a little, 3=Not limited)</p>
</li>
<li>
<p><code>B3B</code> Does your health limit you in moderate activity (1=Limited a lot, 2=Limited a little, 3=Not limited)</p>
</li>
<li>
<p><code>B3C</code> Does health limit you in lift/carry groceries (1=Limited a lot, 2=Limited a little, 3=Not limited)</p>
</li>
<li>
<p><code>B3D</code> Hlth limit you in climb sev stair flights (1=Limited a lot, 2=Limited a little, 3=Not limited)</p>
</li>
<li>
<p><code>B3E</code> Health limit you in climb 1 stair flight (1=Limited a lot, 2=Limited a little, 3=Not limited)</p>
</li>
<li>
<p><code>B3F</code> Health limit you in bend/kneel/stoop (1=Limited a lot, 2=Limited a little, 3=Not limited)</p>
</li>
<li>
<p><code>B3G</code> Does health limit you in walking &gt;1 mile (1=Limited a lot, 2=Limited a little, 3=Not limited)</p>
</li>
<li>
<p><code>B3H</code> Hlth limit you in walking sevrl blocks (1=Limited a lot, 2=Limited a little, 3=Not limited)</p>
</li>
<li>
<p><code>B3I</code> Does health limit you in walking 1 block (1=Limited a lot, 2=Limited a little, 3=Not limited)</p>
</li>
<li>
<p><code>B3J</code> Hlth limit you in bathing/dressing self (1=Limited a lot, 2=Limited a little, 3=Not limited)</p>
</li>
<li>
<p><code>B4A</code> Cut down wrk/act due to phys hlth-lst 4 wks (0=No, 1=Yes)</p>
</li>
<li>
<p><code>B4B</code> Accomplish less due to phys hlth-lst 4 wks (0=No, 1=Yes)</p>
</li>
<li>
<p><code>B4C</code> Lim wrk/act type due to phys hlth-lst 4 wks (0=No, 1=Yes)</p>
</li>
<li>
<p><code>B4D</code> Diff perf work due to phys hlth-lst 4 wks (0=No, 1=Yes)</p>
</li>
<li>
<p><code>B5A</code> Cut wrk/act time due to emot prbs-lst 4 wks (0=No, 1=Yes)</p>
</li>
<li>
<p><code>B5B</code> Accomplish ess due to emot probs-lst 4 wks (0=No, 1=Yes)</p>
</li>
<li>
<p><code>B5C</code> &lt;carefl w/wrk/act due to em prb-lst 4 wks (0=No, 1=Yes)</p>
</li>
<li>
<p><code>B6</code> Ext phys/em intf w/norm soc act-lst 4 wk (1-Not al all, 2=Slightly, 3=Moderately, 4=Quite a bit, 5=Extremely)</p>
</li>
<li>
<p><code>B7</code> Amount of bodily pain-past 4 wks (1=None, 2=Very mild, 3= Mild, 4=Moderate, 5= Severe, 6= Very severe)</p>
</li>
<li>
<p><code>B8</code> Amt pain interf with norm work-last 4 wks (1=Not at all, 2=A little bit, 3=Moderately, 4=Quite a bit, 5=Extremely</p>
</li>
<li>
<p><code>B9A</code> Did you feel full of pep-past 4 wks (1=All of the time, 2=Most of the time, 3 = Good bit of the time, 4=Some of the time, 5=A little of time, 6=None of the time)</p>
</li>
<li>
<p><code>B9B</code> Have you been nervous-past 4 wks (1=All of the time, 2=Most of the time, 3 = Good bit of the time, 4=Some of the time, 5=A little of time, 6=None of the time)</p>
</li>
<li>
<p><code>B9C</code> Felt nothing could cheer you-lst 4 wks (1=All of the time, 2=Most of the time, 3 = Good bit of the time, 4=Some of the time, 5=A little of time, 6=None of the time)</p>
</li>
<li>
<p><code>B9D</code> Have you felt calm/peaceful-past 4 wks (1=All of the time, 2=Most of the time, 3 = Good bit of the time, 4=Some of the time, 5=A little of time, 6=None of the time)</p>
</li>
<li>
<p><code>B9E</code> Did you have a lot of energy-past 4 wks (1=All of the time, 2=Most of the time, 3 = Good bit of the time, 4=Some of the time, 5=A little of time, 6=None of the time)</p>
</li>
<li>
<p><code>B9F</code> Did you feel downhearted-past 4 wks (1=All of the time, 2=Most of the time, 3 = Good bit of the time, 4=Some of the time, 5=A little of time, 6=None of the time)</p>
</li>
<li>
<p><code>B9G</code> Did you feel worn out-past 4 wks (1=All of the time, 2=Most of the time, 3 = Good bit of the time, 4=Some of the time, 5=A little of time, 6=None of the time)</p>
</li>
<li>
<p><code>B9H</code> Have you been a happy pers-past 4 wks (1=All of the time, 2=Most of the time, 3 = Good bit of the time, 4=Some of the time, 5=A little of time, 6=None of the time)</p>
</li>
<li>
<p><code>B9I</code> Did you feel tired-past 4 wks (1=All of the time, 2=Most of the time, 3 = Good bit of the time, 4=Some of the time, 5=A little of time, 6=None of the time)</p>
</li>
<li>
<p><code>B10</code> Amyphys/em prb intf w/soc act-lst 4 wks (1All of the time, 2=Most of the time, 3=Some of the time, 4= A lttle of time, 5= Non of the time)</p>
</li>
<li>
<p><code>B11A</code> I seem to get sick easier than oth peop (1=Definitely true, 2=Mostly True, 3=Don't know, 4=Mostly false, 5=Definitely false)</p>
</li>
<li>
<p><code>B11B</code> I am as healthy as anybody I know (1=Definitely true, 2=Mostly true, 3=Don't know, 4=Mostly false, 5=Definitely False)</p>
</li>
<li>
<p><code>B11C</code> I expect my health to get worse (1=Definitely true, 2=Mostly true, 3=Don't know, 3=Mostly false, 5=Definitely false)</p>
</li>
<li>
<p><code>B11D</code> My health is excellent (1=Definitely true, 2=Mostly true, 3=Don't know, 4=Mostly false, 5=Definitely false)</p>
</li>
<li>
<p><code>C1A</code> Tolf by MD had seix, epil, convuls (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C1B</code> Told by MD had asth, emphys, chr lung dis (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C1C</code> Told by MD had MI (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C1D</code> Told by MD had CHF (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C1E</code> Told by MD had other heart dis (req med) (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C1F</code> Told by MD had HBP (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C1G</code> Told by MD had chronic liver disease (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C1H</code> Told by MD had kidney failure (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C1I</code> Told by MD had chronic art, osteoarth (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C1J</code> Told by MD had peripheral neuropathy (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C1K</code> Ever told by MD had cancer (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C1L</code> Ever told by MD had diabetes (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C1M</code> Ever told by MD had stroke (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2A1</code> Have you ever had skin infections (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2A2</code> Have you had skin infections-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2B1</code> Have you ever had pneumonia (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2B2</code> Have you had pneumonia-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2C1</code> Have you ever had septic arthritis (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2C2</code> Have you had septic arthritis-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2D1</code> Have you ever had TB (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2D2</code> Have you had TB-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2E1</code> Have you ever had endocarditis (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2E2</code> Have you had endocarditis-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2F1</code> Have you ever had an ulcer (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2F2</code> Have you had an ulcer-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2G1</code> Have you ever had pancreatitis (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2G2</code> Have you had pancreatitis-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2H1</code> Ever had abdom pain req overnt hosp stay (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2H2</code> Abdom pain req ovrnt hosp stay-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2I1</code> Have you ever vomited blood (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2I2</code> Have you vomited blood-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2J1</code> Have you ever had hepatitis (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2J2</code> Have you had hepatitis-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2K1</code> Ever had blood clots in legs/lungs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2K2</code> Blood clots in legs/lungs-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2L1</code> Have you ever had osteomyelitis (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2L2</code> Have you had osteomyelitis-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2M1</code> Chst pain using cocaine req ER/hosp (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2M2</code> Chst pain using coc req ER/hosp-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2N1</code> Have you ever had jaundice (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2N2</code> Have you had jaundice-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2O1</code> Lower back pain &gt; 3mos req med attn (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2O2</code> Lwr bck pain &gt;3mos req med attn-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2P1</code> Ever had seizures or convulsions (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2P2</code> Had seizures or convulsions-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2Q1</code> Ever had drug/alc overdose req ER attn (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2Q2</code> Drug/alc overdose req ER attn (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2R1</code> Have you ever had a gunshot wound (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2R2</code> Had a gunshot wound-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2S1</code> Have you ever had a stab wound (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2S2</code> Have you had a stab wound-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2T1</code> Ever had accid/falls req med attn (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2T2</code> Had accid/falls req med attn-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2U1</code> Ever had fract/disloc to bones/joints (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2U2</code> Fract/disloc to bones/joints-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2V1</code> Ever had injury from traffic accident (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2V2</code> Had injury from traffic accid-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2W1</code> Have you ever had a head injury (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C2W2</code> Have you had a head injury-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3A1</code> Have you ever had syphilis (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3A2</code> # times had syphilis</p>
</li>
<li>
<p><code>C3A3</code> Have you had syphilis in last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3B1</code> Have you ever had gonorrhea (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3B2</code> # times had gonorrhea</p>
</li>
<li>
<p><code>C3B3</code> Have you had gonorrhea in last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3C1</code> Have you ever had chlamydia (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3C2</code> # of times had Chlamydia</p>
</li>
<li>
<p><code>C3C3</code> Have you had chlamydia in last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3D</code> Have you ever had genital warts (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3E</code> Have you ever had genital herpes (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3F1</code> Have you ever had other STD's (not HIV) (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3F2</code> # of times had other STD's (not HIV)</p>
</li>
<li>
<p><code>C3F3</code> Had other STD's (not HIV)-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3F_T</code> a factor with levels <code>7</code> <code>CRABS</code> <code>CRABS - TRICHONOMIS</code> <code>CRABS, HEP B</code> <code>DOESNT KNOW NAME</code> <code>HAS HAD ALL 3 ABC</code> <code>HEP B</code> <code>HEP B, TRICAMONAS</code> <code>HEP. B</code> <code>HEPATITIS B</code> <code>HEPATITS B</code> <code>TRICHAMONAS VAGINALA</code> <code>TRICHAMONIS</code> <code>TRICHOMONAS</code> <code>TRICHOMONIASIS</code> <code>TRICHOMONIS</code> <code>TRICHOMONIS VAGINITI</code> <code>TRICHOMORAS</code> <code>TRICHONOMIS</code></p>
</li>
<li>
<p><code>C3G1</code> Have you ever been tested for HIV/AIDS (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3G2</code> # times tested for HIV/AIDS</p>
</li>
<li>
<p><code>C3G3</code> Have you been tested for HIV/AIDS-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3G4</code> What was the result of last test (1=Positive, 2=Negative, 3=Refued, 4=Never got result, 5=Inconclusive</p>
</li>
<li>
<p><code>C3H1</code> Have you ever had PID (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3H2</code> # of times had PID</p>
</li>
<li>
<p><code>C3H3</code> Have you had PID in last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3I</code> Have you ever had a Pap smear (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3J</code> Have you had a Pap smear in last 3 years (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3K</code> Are you pregnant (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C3K_M</code> How many mos pregnant</p>
</li>
<li>
<p><code>D1</code> $ of times hospitalized for med probs</p>
</li>
<li>
<p><code>D2</code> Take prescr med regularly for phys prob (0=No, 1=Yes)</p>
</li>
<li>
<p><code>D3</code> # days had med probs-30 days bef detox</p>
</li>
<li>
<p><code>D4</code> How bother by med prob-30days bef detox (0=Not at all, 1=Slightly, 2=Moderately, 3=Considerably, 4=Extremely)</p>
</li>
<li>
<p><code>D5</code> How import is trtmnt for these med probs (0=Not at all, 1=Slightly, 2= Moderately, 3= Considerably, 4= Extremely</p>
</li>
<li>
<p><code>E2A</code> Detox prog for alc or drug prob-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E2B</code> # times entered a detox prog-lst 6 mos</p>
</li>
<li>
<p><code>E2C</code> # nights ovrnight in detox prg-lst 6 mos</p>
</li>
<li>
<p><code>E3A</code> Holding unit for drug/alc prob-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E3B</code> # times in holding unity=lst 6 mos</p>
</li>
<li>
<p><code>E3C</code> # total nights in holding unit-lst 6 mos</p>
</li>
<li>
<p><code>E4A</code> In halfway hse/resid facil-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E4B</code> # times in hlfwy hse/res facil-lst 6 mos</p>
</li>
<li>
<p><code>E4C</code> Ttl nites in hlfwy hse/res fac-last 6 mos</p>
</li>
<li>
<p><code>E5A</code> In day trtmt prg for alcohol/drug-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E5B</code> Total # days in day trtmt prg-lst 6 mos</p>
</li>
<li>
<p><code>E6</code> In methadone maintenance prg-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E7A</code> Visit outpt prg subst ab couns-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E7B</code> # visits outpt prg subst ab couns-lst 6 mos</p>
</li>
<li>
<p><code>E8A1</code> Saw MD/H care wkr re alcohol/drugs-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E8A2</code> Saw Prst/Min/Rabbi re alcohol/drugs-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E8A3</code> Employ Asst Prg for alcohol/drug prb-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E8A4</code> Oth source cnsl for alcohol/drug prb-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E9A</code> AA/NA/slf-hlp for drug/alcohol/emot-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E9B</code> How often attend AA/NA/slf-hlp-lst 6 mos (1=Daily, 2=2-3 Times/week, 3=Weekly, 4=Every 2 weeks, 5=Once/month</p>
</li>
<li>
<p><code>E10A</code> have you been to med clinic-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E10B1</code> # x visit ment hlth clin/prof-lst 6 mos</p>
</li>
<li>
<p><code>E10B2</code> # x visited med clin/priv MD-lst 6 mos</p>
</li>
<li>
<p><code>E10C19</code> Visited private MD-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E11A</code> Did you stay ovrnite/+ in hosp-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E11B</code> # times ovrnight/+ in hosp-last 6 mos</p>
</li>
<li>
<p><code>E11C</code> Total # nights in hosp-last 6 mos</p>
</li>
<li>
<p><code>E12A</code> Visited Hosp ER for med care-past 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E12B</code> # times visited hosp ER-last 6 mos</p>
</li>
<li>
<p><code>E13</code> Tlt # visits to MDs-lst 2 wks bef detox</p>
</li>
<li>
<p><code>E14A</code> Recd trtmt from acupuncturist-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E14B</code> Recd trtmt from chiropractor-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E14C</code> Trtd by hol/herb/hom med prac-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E14D</code> Recd trtmt from spirit healer-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E14E</code> Have you had biofeedback-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E14F</code> Have you underwent hypnosis-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E14G</code> Received other treatment-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E15A</code> Tried to get subst ab services-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E15B</code> Always able to get subst ab servies (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E15C1</code> I could not pay for services (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E15C2</code> I did not know where to go for help (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E15C3</code> Couldn't get to services due to transp prob (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E15C4</code> The offie/clinic hrs were inconvenient (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E15C5</code> Didn't speak/understnd Englsh well enough (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E15C6</code> Afraid other might find out about prob (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E15C7</code> My substance abuse interfered (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E15C8</code> Didn't have someone to watch my children (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E15C9</code> I did not want to lose my job (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E15C10</code> My insurance didn't cover services (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E15C11</code> There were no beds available at the prog (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E15C12</code> Other reason not get sub ab services (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A1</code> I cannot pay for services (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A2</code> I am not eligible for free care (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A3</code> I do not know where to go (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A4</code> Can't get to services due to trans prob (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A5</code> a numeric vectorOffice/clinic hours are inconvenient (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A6</code> I don't speak/understnd enough English (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A7</code> Afraid othrs find out about my hlth prob (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A8</code> My substance abuse interferes (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A9</code> I don't have someone to watch my childrn (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A10</code> I do not want to lose my job (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A11</code> My insurance doesn't cover charges (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A12</code> I do not feel I need a regular MD (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A13</code> Other reasons don't have regular MD (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E18A</code> I could not pay for services (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E18B</code> I did not know where to go for help (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E18C</code> Couldn't get to services due to transp prob (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E18D</code> The office/clinic hrs were inconvenient (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E18F</code> Afraid others might find out about prob (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E18G</code> My substance abuse interfered (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E18H</code> Didn't have someone to watch my children (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E18I</code> I did not want to lose my job (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E18J</code> My insurance didn't cover services (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E18K</code> There were no beds available at the prog (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E18L</code> I do not need substance abuse services (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E18M</code> Other reason not get sub ab services (0=No, 1=Yes)</p>
</li>
<li>
<p><code>F1A</code> Bothered by thngs not gen boethered by (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1B</code> My appretite was poor (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1C</code> Couldn't shake blues evn w/fam+frnds hlp (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1D</code> Felt I was just as good as other people (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1E</code> Had trouble keeping mind on what doing (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1F</code> I felt depressed (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1G</code> I felt everthing I did was an effort (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1H</code> I felt hopeful about the future (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1I</code> I thought my life had been a failure (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1J</code> I felt fearful (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1K</code> My sleep was restless (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1L</code> I was happy (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1M</code> I talked less than usual (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1N</code> I felt lonely (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1O</code> People were unfriendly (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1P</code> I enoyed life (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1Q</code> I had crying spells (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1R</code> I felt sad (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1S</code> I felt that people dislike me (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>F1T</code> I could not get going (0=Rarely/never, 1=Some of the time, 2=Occas/moderately, 3=Most of the time)</p>
</li>
<li>
<p><code>G1A</code> Diff contr viol beh for sig time per evr (0=No, 1=Yes)</p>
</li>
<li>
<p><code>G1A_30</code> Diff contr viol beh-sig per lst 30 days (0=No, 1=Yes)</p>
</li>
<li>
<p><code>G1B</code> Ever had thoughts of suicide (0=No, 1=Yes)</p>
</li>
<li>
<p><code>G1B_30</code> Had thoughts of suicide-lst 30 days (0=No, 1=Yes)</p>
</li>
<li>
<p><code>G1C</code> Attempted suicide ever (0=No, 1=Yes)</p>
</li>
<li>
<p><code>G1C_30</code> Attempted suicide-lst 30 days (0=No, 1=Yes)</p>
</li>
<li>
<p><code>G1D</code> Prescr med for pst/emot prob ever (0=No, 1=Yes)</p>
</li>
<li>
<p><code>G1D_30</code> Prescr med for psy/emot prob-lst 30 days (0=No, 1=Yes)</p>
</li>
<li>
<p><code>H1_30</code> # days in past 30 bef detox used alcohol</p>
</li>
<li>
<p><code>H1_LT</code> # yrs regularly used alcohol</p>
</li>
<li>
<p><code>H1_RT</code> Route of administration use alcohol (0=N/A. 1=Oral, 2=Nasal, 3=Smoking, 4=Non-IV injection, 5=IV)</p>
</li>
<li>
<p><code>H2_30</code> #days in 3- bef detox use alc to intox</p>
</li>
<li>
<p><code>H2_LT</code> # yrs regularly used alcohol to intox</p>
</li>
<li>
<p><code>H2_RT</code> Route of admin use alcohol to intox (0=N/A. 1=Oral, 2=Nasal, 3=Smoking, 4=Non-IV injection, 5=IV)</p>
</li>
<li>
<p><code>H3_30</code> # days in past 30 bef detox used heroin</p>
</li>
<li>
<p><code>H3_LT</code> # yrs regularly used heroin</p>
</li>
<li>
<p><code>H3_RT</code> Route of administration of heroin (0=N/A. 1=Oral, 2=Nasal, 3=Smoking, 4=Non-IV injection, 5=IV)</p>
</li>
<li>
<p><code>H4_30</code> # days used methadone-lst 30 bef detox</p>
</li>
<li>
<p><code>H4_LT</code> # yrs regularly used methadone</p>
</li>
<li>
<p><code>H4_RT</code> Route of administration of methadone (0=N/A. 1=Oral, 2=Nasal, 3=Smoking, 4=Non-IV injection, 5=IV)</p>
</li>
<li>
<p><code>H5_30</code> # days used opi/analg-lst 30 bef detox</p>
</li>
<li>
<p><code>H5_LT</code> # yrs regularly used oth opiates/analg</p>
</li>
<li>
<p><code>H5_RT</code> Route of admin of oth opiates/analg (0=N/A. 1=Oral, 2=Nasal, 3=Smoking, 4=Non-IV injection, 5=IV)</p>
</li>
<li>
<p><code>H6_30</code> # days in past 30 bef detox used barbit</p>
</li>
<li>
<p><code>H6_LT</code> # yrs regularly used barbiturates</p>
</li>
<li>
<p><code>H6_RT</code> Route of admin of barbiturates (0=N/A. 1=Oral, 2=Nasal, 3=Smoking, 4=Non-IV injection, 5=IV)</p>
</li>
<li>
<p><code>H7_30</code> # days used sed/hyp/trnq-lst 30 bef det</p>
</li>
<li>
<p><code>H7_LT</code> # yrs regularly used sed/hyp/trnq</p>
</li>
<li>
<p><code>H7_RT</code> Route of admin of sed/hyp/trnq (0=N/A. 1=Oral, 2=Nasal, 3=Smoking, 4=Non-IV injection, 5=IV)</p>
</li>
<li>
<p><code>H8_30</code> # days in lst 30 bef detox used cocaine</p>
</li>
<li>
<p><code>H8_LT</code> # yrs regularly used cocaine</p>
</li>
<li>
<p><code>H8_RT</code> Route of admin of cocaine (0=N/A. 1=Oral, 2=Nasal, 3=Smoking, 4=Non-IV injection, 5=IV)</p>
</li>
<li>
<p><code>H9_30</code> # days in lst 30 bef detox used amphet</p>
</li>
<li>
<p><code>H9_LT</code> # yrs regularly used amphetamines</p>
</li>
<li>
<p><code>H9_RT</code> Route of admin of amphetamines (0=N/A. 1=Oral, 2=Nasal, 3=Smoking, 4=Non-IV injection, 5=IV)</p>
</li>
<li>
<p><code>H10_30</code> # days in lst 30 bef detox used cannabis</p>
</li>
<li>
<p><code>H10_LT</code> # yrs regularly used cannabis</p>
</li>
<li>
<p><code>H10_RT</code> Route of admin of cannabis (0=N/A. 1=Oral, 2=Nasal, 3=Smoking, 4=Non-IV injection, 5=IV)</p>
</li>
<li>
<p><code>H11_30</code> # days in lst 30 bef detox used halluc</p>
</li>
<li>
<p><code>H11_LT</code> # yrs regularly used hallucinogens</p>
</li>
<li>
<p><code>H11_RT</code> Route of admin of hallucinogens (0=N/A. 1=Oral, 2=Nasal, 3=Smoking, 4=Non-IV injection, 5=IV)</p>
</li>
<li>
<p><code>H12_30</code> # days in lst 30 bef detox used inhalant</p>
</li>
<li>
<p><code>H12_LT</code> # yrs regularly used inhalants</p>
</li>
<li>
<p><code>H12_RT</code> Route of admin of inhalants (0=N/A. 1=Oral, 2=Nasal, 3=Smoking, 4=Non-IV injection, 5=IV)</p>
</li>
<li>
<p><code>H13_30</code> # days used &gt;1 sub/day-lst 30 bef detox</p>
</li>
<li>
<p><code>H13_LT</code> # yrs regularly used &gt;1 subst/day</p>
</li>
<li>
<p><code>H13_RT</code> Route of admin of &gt;1 subst/day (0=N/A. 1=Oral, 2=Nasal, 3=Smoking, 4=Non-IV injection, 5=IV)</p>
</li>
<li>
<p><code>H14</code> Accord to interview w/c subst is main prob (0=No problem, 1=Alcohol, 2=Alcool to intox, 3=Heroin 4=Methadone, 5=Oth opiate/analg, 6=Barbituates, 7=Sed/hyp/tranq, 8=Cocaine, 9=Amphetamines, 10=Marij/cannabis</p>
</li>
<li>
<p><code>H15A</code> # times had alchol DTs</p>
</li>
<li>
<p><code>H15B</code> # times overdosed on drugs</p>
</li>
<li>
<p><code>H16A</code> $ spent on alc-lst 30 days bef detox</p>
</li>
<li>
<p><code>H16B</code> $ spent on drugs-lst 30 days bef detox</p>
</li>
<li>
<p><code>H17A</code> # days had alc prob-lst 30 days bef det</p>
</li>
<li>
<p><code>H17B</code> # days had drug prob-lst 30 days bef det</p>
</li>
<li>
<p><code>H18A</code> How troubled by alc probs-lst 30 days (0=Not at all, 1=Slightly, 2=Moderately, 3=Considerably, 4=Extremely)</p>
</li>
<li>
<p><code>H18B</code> How troubled by drug probs-lst 30 days (0=Not at all, 1=Slightly, 2=Moderately, 3=Considerably, 4=Extremely)</p>
</li>
<li>
<p><code>H19A</code> How import is trtmnt for alc probs now (0=Not at all, 1=Slightly, 2=Moderately, 3=Considerably, 4=Extremely)</p>
</li>
<li>
<p><code>H19B</code> How importy is trtmnt for drug probs now (0=Not at all, 1=Slightly, 2=Moderately, 3=Considerably, 4=Extremely)</p>
</li>
<li>
<p><code>I1</code> Avg # drinks in lst 30 days bef detox</p>
</li>
<li>
<p><code>I2</code> Most drank any 1 day in lst 30 bef detox</p>
</li>
<li>
<p><code>I3</code> On days used heroin, avg # bags used</p>
</li>
<li>
<p><code>I4</code> Most bgs heroin use any 1 day-30 bef det</p>
</li>
<li>
<p><code>I5</code> Avg $ amt of heorin used per day</p>
</li>
<li>
<p><code>I6A</code> On days used cocaine, avg # bags used</p>
</li>
<li>
<p><code>I6B</code> On days used cocaine, avg # rocks used</p>
</li>
<li>
<p><code>I7A</code> Mst bgs cocaine use any 1 day-30 bef det</p>
</li>
<li>
<p><code>I7B</code> Mst rcks cocaine use any 1 day-30 bef det</p>
</li>
<li>
<p><code>I8</code> Avg $ amt of cocaine used per day</p>
</li>
<li>
<p><code>J1</code> Evr don't stop using cocaine when should (0=No, 1=Yes)</p>
</li>
<li>
<p><code>J2</code> Ever tried to cut down on cocaine (0=No, 1=Yes)</p>
</li>
<li>
<p><code>J3</code> Does cocaine take up a lot of your time (0=No, 1=Yes)</p>
</li>
<li>
<p><code>J4</code> Need use &gt; cocaine to get some feeling (0=No, 1=Yes)</p>
</li>
<li>
<p><code>J5A</code> Get phys sick when stop using cocaine (0=No, 1=Yes)</p>
</li>
<li>
<p><code>J5B</code> Ever use cocaine to prevent getting sick (0=No, 1=Yes)</p>
</li>
<li>
<p><code>J6</code> Ever don't stop using heroin when should (0=No, 1=Yes)</p>
</li>
<li>
<p><code>J7</code> Ever tried to cut down on heroin (0=No, 1=Yes)</p>
</li>
<li>
<p><code>J8</code> Does heroin take up a lot of your time (0=No, 1=Yes)</p>
</li>
<li>
<p><code>J9</code> Need use &gt; heroin to get some feeling (0=No, 1=Yes)</p>
</li>
<li>
<p><code>J10A</code> Get phys sick when stop using heroin (0=No, 1=Yes)</p>
</li>
<li>
<p><code>J10B</code> Ever use heroin to prevent getting sick (0=No, 1=Yes)</p>
</li>
<li>
<p><code>K1</code> Do you currently smoke cigarettes (1=Yes-every day, 2=Yes-some days, 3=No-former smoker, 4=No-never&gt;100 cigs</p>
</li>
<li>
<p><code>K2</code> Avg # cigarettes smoked per day</p>
</li>
<li>
<p><code>K3</code> Considering quitting cigs w/in next 6 mo (0=No, 1=Yes)</p>
</li>
<li>
<p><code>L1</code> How often drink last time drank (1=To get high/less, 2=To get drunk, 3=To pass out)</p>
</li>
<li>
<p><code>L2</code> Often have hangovrs Sun or Mon mornings (0=No, 1=Yes)</p>
</li>
<li>
<p><code>L3</code> Have you had the shakes when sobering (0=No, 1=Sometimes, 2=Alm evry time drink)</p>
</li>
<li>
<p><code>L4</code> Do you get phys sick as reslt of drinking (0=No, 1=Sometimes, 2=Alm evry time drink)</p>
</li>
<li>
<p><code>L5</code> have you had the DTs (0=No, 1=Once, 2=Several times</p>
</li>
<li>
<p><code>L6</code> When drink do you stumble/stagger/weave (0=No, 1=Sometimes, 2=Often)</p>
</li>
<li>
<p><code>L7</code> D/t drinkng felt overly hot/sweaty (0=No, 1=Once, 2=Several times)</p>
</li>
<li>
<p><code>L8</code> As result of drinkng saw thngs not there (0=No, 1=Once, 2=Several times)</p>
</li>
<li>
<p><code>L9</code> Panic because fear not have drink if need it (0=No, 1=Yes)</p>
</li>
<li>
<p><code>L10</code> Have had blkouts as result of drinkng (0=No, never, 1=Sometimes, 2=Often, 3=Alm evry time drink)</p>
</li>
<li>
<p><code>L11</code> Do you carry bottle or keep close by (0=No, 1=Some of the time, 2=Most of the time)</p>
</li>
<li>
<p><code>L12</code> After abstin end up drink heavily again (0=No, 1=Sometimes, 2=Almost evry time)</p>
</li>
<li>
<p><code>L13</code> Passed out due to drinking-lst 12 mos (0=No, 1=Once, 2=More than once)</p>
</li>
<li>
<p><code>L14</code> Had convuls following period of drinkng (0=No, 1=Once, 2=Several times)</p>
</li>
<li>
<p><code>L15</code> Do you drink throughout the day (0=No, 1=Yes)</p>
</li>
<li>
<p><code>L16</code> Aftr drinkng heavily was thinkng unclear (0=No, 1=Yes, few hrs, 2=Yes,1-2 days, 3=Yes, many days)</p>
</li>
<li>
<p><code>L17</code> D/t drinkng felt heart beat rapidly (0=No, 1=Once, 2=Several times)</p>
</li>
<li>
<p><code>L18</code> Do you constntly think about drinkng/alc (0=No, 1=Yes)</p>
</li>
<li>
<p><code>L19</code> D/t drinkng heard things not there (0=No, 1=Once, 2= Several times)</p>
</li>
<li>
<p><code>L20</code> Had weird/fright sensations when drinkng (0=No, 1=Once or twice, 2=Often)</p>
</li>
<li>
<p><code>L21</code> When drinkng felt things rawl not there (0=No, 1=Once, 2=Several times)</p>
</li>
<li>
<p><code>L22</code> With respect to blackouts (0=Never had one, 1=Had for &lt;1hr, 2=Had several hrs, 3=Had for day/+)</p>
</li>
<li>
<p><code>L23</code> Ever tried to cut down on drinking &amp; failed (0=No, 1=Once, 2=Several times)</p>
</li>
<li>
<p><code>L24</code> Do you gulp drinks (0=No, 1=Yes)</p>
</li>
<li>
<p><code>L25</code> After taking 1 or 2 drinks can you stop (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M1</code> Had hangover/felt bad aftr using alcohol/drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M2</code> Felt bad about self because of alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M3</code> Missed days wrk/sch because of alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M4</code> Fam/frinds worry/compl about alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M5</code> I have enjoyed drinking/using drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M6</code> Qual of work suffered because of alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M7</code> Parenting ability harmed by alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M8</code> Trouble sleeping/nightmares aftr alcohol/drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M9</code> Driven motor veh while undr inf alcohol/drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M10</code> Using alcohol/1 drug caused &gt; use othr drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M11</code> I have been sick/vomited aft alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M12</code> I have been unhappy because of alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M13</code> Lost weight/eaten poorly due to alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M14</code> Fail to do what expected due to alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M15</code> Using alcohol/drugs has helped me to relax (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M16</code> Felt guilt/ashamed because of my alc drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M17</code> Said/done emarras thngs when on alcohol/drug (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M18</code> Personality changed for worse on alcohol/drug (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M19</code> Taken foolish risk when using alcohol/drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M20</code> Gotten into trouble because of alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M21</code> Said cruel things while using alcohol/drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M22</code> Done impuls thngs regret due to alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M23</code> Gotten in phys fights when use alcohol/drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M24</code> My phys health was harmed by alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M25</code> Using alcohol/drug helped me have more + outlook (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M26</code> I have had money probs because of my alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M27</code> My love relat harmed due to my alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M28</code> Smoked tobacco more when using alcohol/drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M29</code> &lt;y phys appearance harmed by alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M30</code> My family hurt because of my alc drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M31</code> Close relationsp damaged due to alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M32</code> Spent time in jail because of my alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M33</code> My sex life suffered due to my alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M34</code> Lost interst in activity due to my alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M35</code> Soc life&gt; enjoyable when using alcohol/drug (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M36</code> Spirit/moral life harmed by alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M37</code> Not had kind life want due to alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M38</code> My alcohol/drug use in way of personal growth (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M39</code> My alcohol/drug use damaged soc life/reputat (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M40</code> Spent/lost too much $ because alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M41</code> Arrested for DUI of alc or oth drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M42</code> Arrested for offenses rel to alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M43</code> Lost marriage/love relat due to alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M44</code> Susp/fired/left job/sch due to alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M45</code> I used drugs moderately w/o having probs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M46</code> I have lost a friend due to my alcohol/drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M47</code> Had an accident while using alcohol/drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M48</code> Phys hurt/inj/burned when using alcohol/drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M49</code> I injured someone while using alcohol/drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>M50</code> Damaged things/prop when using alcohol/drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N1A</code> My friends give me the moral support I need (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N1B</code> Most people closer to friends than I am (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N1C</code> My friends enjoy hearing what I think (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N1D</code> I rely on my friends for emot support (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N1E</code> Friend go to when down w/o feel funny later (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N1F</code> Frnds and I open re what thnk about things (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N1G</code> My friends sensitive to my pers needs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N1H</code> My friends good at helping me solve probs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N1I</code> have deep sharing relat w/ a # of frnds (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N1J</code> When confide in frnds makes me uncomfort (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N1K</code> My friends seek me out for companionship (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N1L</code> Not have as int relat w/frnds as others (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N1M</code> Recent good idea how to do somethng frm frnd (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N1N</code> I wish my friends were much different (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N2A</code> My family gives me the moral support I need (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N2B</code> Good ideas of how do/make thngs from fam (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N2C</code> Most peop closer to their fam than I am (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N2D</code> When confide make close fam membs uncomf (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N2E</code> My fam enjoys hearing about what I think (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N2F</code> Membs of my fam share many of my intrsts (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N2G</code> I rely on my fam for emot support (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N2H</code> Fam memb go to when down w/o feel funny (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N2I</code> Fam and I open about what thnk about thngs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N2J</code> My fam is sensitive to my personal needs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N2K</code> Fam memb good at helping me solve probs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N2L</code> Have deep sharing relat w/# of fam membs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N2M</code> Makes me uncomf to confide in fam membs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>N2N</code> I wish my family were much different (0=No, 1=Yes)</p>
</li>
<li>
<p><code>O1A</code> # people spend tx w/who drink alc (1=None, 2= A few, 3=About half, 4= Most, 5=All)</p>
</li>
<li>
<p><code>O1B</code> # people spend tx w/who are heavy drinkrs (1=None, 2= A few, 3=About half, 4= Most, 5=All)</p>
</li>
<li>
<p><code>O1C</code> # people spend tx w/who use drugs (1=None, 2= A few, 3=About half, 4= Most, 5=All)</p>
</li>
<li>
<p><code>O1D</code> # peop spend tx w/who supprt your abstin (1=None, 2= A few, 3=About half, 4= Most, 5=All)</p>
</li>
<li>
<p><code>O2</code> Does live-in part/spouse drink/use drugs (0=No, 1=Yes, 2=N/A)</p>
</li>
<li>
<p><code>P1A</code> Phys abuse/assaul by fam memb/pers know (0=No, 1=Yes, 7=Not sure)</p>
</li>
<li>
<p><code>P1B</code> Age first phys assaulted by pers know</p>
</li>
<li>
<p><code>P1C</code> Phys assaulted by pers know-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>P2A</code> Phys abuse/assaul by stranger (0=No, 1=Yes, 7=Not sure)</p>
</li>
<li>
<p><code>P2B</code> Age first phys assaulted by stranger</p>
</li>
<li>
<p><code>P2C</code> Phys assaulted by stranger-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>P3</code> Using drugs/alc when phys assaulted (1=Don't know, 2=Never, 3=Some cases, 4=Most cases, 5=All cases, 9=Never assaulted)</p>
</li>
<li>
<p><code>P4</code> Pers who phys assault you using alcohol/drugs (1=Don't know, 2=Never, 3=Some cases, 4=Most cases, 5=All cases, 9=Never assaulted)</p>
</li>
<li>
<p><code>P5A</code> Sex abuse/assual by fam memb/pers know (0=No, 1= Yes, 7=Not sure)</p>
</li>
<li>
<p><code>P5B</code> Age first sex assaulted by pers know</p>
</li>
<li>
<p><code>P5C</code> Sex assaulted by pers know-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>P6A</code> Sex abuse/assaul by stranger (0=No, 1=Yes, 7=Not sure)</p>
</li>
<li>
<p><code>P6B</code> Age first sex assaulted by stranger</p>
</li>
<li>
<p><code>P6C</code> Sex assaulted by stranger-last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>P7</code> Using drugs/alc when sex assaulted (1=Don't know, 2=Never, 3=Some cases, 4=Most cases, 5=All cases, 9=Never assaulted)</p>
</li>
<li>
<p><code>P8</code> Person who sex assaulted you using alcohol/drugs (1=Don't know, 2=Never, 3=Some cases, 4=Most cases, 5=All cases, 9=Never assaulted)</p>
</li>
<li>
<p><code>Q1A</code> Have you ever injected drugs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>Q1B</code> Have you injected drugs-lst 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>Q2</code> Have you shared needles/works-last 6 mos (0=No/Not shot up, 3=Yes)</p>
</li>
<li>
<p><code>Q3</code> # people shared needles w/past 6 mos (0=No/Not shot up, 1=1 other person, 2=2-3 diff people, 3=4/+ diff people)</p>
</li>
<li>
<p><code>Q4</code> How often been to shoot gall/hse-lst 6 mos (0=Never, 1=Few times or less, 2= Few times/month, 3= Once or more/week)</p>
</li>
<li>
<p><code>Q5</code> How often been to crack house-last 6 mos (0=Never, 1=Few times or less, 2=Few times/month, 3=Once or more/week)</p>
</li>
<li>
<p><code>Q6</code> How often shared rinse-water-last 6 mos (0=Nevr/Not shot up, 1=Few times or less, 2=Few times/month, 3=Once or more/week)</p>
</li>
<li>
<p><code>Q7</code> How often shared a cooker-last 6 mos (0=Nevr/Not shot up, 1=Few times or less, 2=Few times/month, 3=Once or more/week)</p>
</li>
<li>
<p><code>Q8</code> How often shared a cotton-last 6 mos (0=Nevr/Not shot up, 1=Few times or less, 2=Few times/month, 3=Once or more/week)</p>
</li>
<li>
<p><code>Q9</code> How often use syringe to div drugs-lst 6 mos (0=Nevr/Not shot up, 1=Few times or less, 2=Few times/month, 3=Once or more/week)</p>
</li>
<li>
<p><code>Q10</code> How would you describe yourself (0=Straight, 1=Gay/bisexual)</p>
</li>
<li>
<p><code>Q11</code> # men had sex w/in past 6 months (0=0 men, 1=1 man, 2=2-3 men, 3=4+ men</p>
</li>
<li>
<p><code>Q12</code> # women had sex w/in past 6 months (0=0 women, 1=1woman, 2=2-3 women, 3=4+ women</p>
</li>
<li>
<p><code>Q13</code> # times had sex In past 6 mos (0=Never, 1=Few times or less, 2=Few times/month, 3=Once or more/week)</p>
</li>
<li>
<p><code>Q14</code> How often had sex to get drugs-last 6 mos (0=Never, 1=Few times or less, 2=Few times/month, 3=Once or more/week)</p>
</li>
<li>
<p><code>Q15</code> How often given drugs to have sex-lst 6 mos (0=Never, 1=Few times or less, 2=Few times/month, 3=Once or more/week)</p>
</li>
<li>
<p><code>Q16</code> How often were you paid for sex-lst 6 mos (0=Never, 1=Few times or less, 2=Few times/month, 3=Once or more/week)</p>
</li>
<li>
<p><code>Q17</code> How often you pay pers for sex-lst 6 mos (0=Never, 1=Few times or less, 2=Few times/month, 3=Once or more/week)</p>
</li>
<li>
<p><code>Q18</code> How often use condomes during sex=lst 6 mos (0=No sex/always, 1=Most of the time, 2=Some of the time, 3=None of the time)</p>
</li>
<li>
<p><code>Q19</code> Condoms are too much of a hassle to use (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>Q20</code> Safer sex is always your responsibility (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1A</code> I really want to hange my alcohol/drug use (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1B</code> Sometimes I wonder if I'm an alcohol/addict (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1C</code> Id I don't chng alcohol/drug probs will worsen (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1D</code> I started making changes in alcohol/drug use (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1E</code> Was using too much but managed to change (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1F</code> I wonder if my alcohol/drug use hurting othrs (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1G</code> I am a prob drinker or have drug prob (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1H</code> Already doing thngs to chnge alcohol/drug use (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1I</code> have changed use-trying to not slip back (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1J</code> I have a serious problem w/ alcohol/drugs (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1K</code> I wonder if I'm in contrl of alcohol/drug use (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1L</code> My alcohol/drug use is causing a lot of harm (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1M</code> Actively curring down/stopping alcohol/drug use (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1N</code> Want help to not go back to alcohol/drugs (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1O</code> I know that I have an alcohol/drug problem (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1P</code> I wonder if I use alcohol/drugs too much (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1Q</code> I am an alcoholic or drug addict (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1R</code> I am working hard to change alcohol/drug use (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>R1S</code> Some changes-want help from going back (1=Strongly disagree, 2=Disagree, 3= Agree, 4=Strongly agree)</p>
</li>
<li>
<p><code>S1A</code> At interview pt obviously depressed/withdrawn (0=No, 1=Yes)</p>
</li>
<li>
<p><code>S1B</code> at interview pt obviously hostile (0=No, 1=Yes)</p>
</li>
<li>
<p><code>S1C</code> At interview pt obviouslt anx/nervous (0=No, 1=Yes)</p>
</li>
<li>
<p><code>S1D</code> Trouble w/real tst/thght dis/par at interview (0=No, 1=Yes)</p>
</li>
<li>
<p><code>S1E</code> At interview pt trbl w/ compr/concen/rememb (0=No, 1=Yes)</p>
</li>
<li>
<p><code>S1F</code> At interview pt had suicidal thoughts (0=No, 1=Yes)</p>
</li>
<li>
<p><code>T1</code> Have used alc since leaving River St. (0=No, 1=Yes)</p>
</li>
<li>
<p><code>T1B</code> # days in row continued to drink</p>
</li>
<li>
<p><code>T1C</code> Longest period abstain-lst 6 mos (alc)</p>
</li>
<li>
<p><code>T2</code> Have used heroin since leaving River St (0=No, 1=Yes)</p>
</li>
<li>
<p><code>T2B</code> # days in row continued to use heroin</p>
</li>
<li>
<p><code>T2C</code> Longest period abstain-lst 6 mos (heroin)</p>
</li>
<li>
<p><code>T3</code> Have used cocaine since leaving River St (0=No, 1=Yes)</p>
</li>
<li>
<p><code>T3B</code> # days in row continued to use cocaine</p>
</li>
<li>
<p><code>T3C</code> Lngest period abstain-lst 6 mos (cocaine)</p>
</li>
<li>
<p><code>U1</code> It is important to have a regular MD (1=Strongly agree, 2=Agree, 3=Uncertain, 4=Disagree, 5=Strongly Disagree)</p>
</li>
<li>
<p><code>U2A</code> I cannot pay for services (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2B</code> I am not eligible for free care (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2C</code> I do not know where to go (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2D</code> Can't get services due to transport probs (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2E</code> Office/clinic hours are inconvenient (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2F</code> I do not speak/understand English well (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2G</code> Afraid others discover hlth prb I have (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2H</code> My substance abuse interferes (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2I</code> I do not have a babysitter (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2J</code> I do not want to lose my job (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2K</code> My insurance does not cover services (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2L</code> Medical care is not important to me (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2M</code> I do not have time (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2N</code> Med staff do not treat me with respect (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2O</code> I do not trust my doctors or nurses (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2P</code> Often been unsatisfied w/my med care (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2Q</code> Other reason hard to get regular med care (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U2Q_T</code> a factor with many levels</p>
</li>
<li>
<p><code>U2R</code> a factor with levels <code>7</code> <code>A</code> <code>B</code> <code>C</code> <code>D</code> <code>E</code> <code>F</code> <code>G</code> <code>H</code> <code>I</code> <code>J</code> <code>K</code> <code>L</code> <code>M</code> <code>N</code> <code>O</code> <code>P</code> <code>Q</code></p>
</li>
<li>
<p><code>U3A</code> Has MD evr talked to you about drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U3B</code> Has MD evr talked to you about alc use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U4</code> Is there an MD you consider your regular MD (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U5</code> Have you seen any MDs in last 6 mos (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U6A</code> Would you go to this MD if med prb not emer (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U6B</code> Think one of these could be your regular MD (0=No, 1=Yes)</p>
</li>
<li>
<p><code>PCP_ID</code> a numeric vector</p>
</li>
<li>
<p><code>U7A</code> What type of MD is your regular MD/this MD (1=OB/GYN, 2=Family medicine, 3=Pediatrician, 4=Adolescent medicine, 5=Internal medicine, 6=AIDS doctor, 7=Asthma doctor, 8=Pulmonary doctor, 9=Cardiologist, 10=Gastroen)</p>
</li>
<li>
<p><code>U7A_T</code> a factor with levels <code>ARTHRITIS DOCTOR</code> <code>CHIROPRACTOR</code> <code>COCAINE STUDY</code> <code>DETOX DOCTOR</code> <code>DO</code> <code>EAR DOCTOR</code> <code>EAR SPECIALIST</code> <code>EAR, NOSE, &amp; THROAT.</code> <code>EAR/NOSE/THROAT</code> <code>ENT</code> <code>FAMILY PHYSICIAN</code> <code>GENERAL MEDICINE</code> <code>GENERAL PRACTICE</code> <code>GENERAL PRACTIONER</code> <code>GENERAL PRACTITIONER</code> <code>HEAD &amp; NECK SPECIALIST</code> <code>HERBAL/HOMEOPATHIC/ACUPUNCTURE</code> <code>ID DOCTOR</code> <code>MAYBE GENERAL PRACTITIONER</code> <code>MEDICAL STUDENT</code> <code>NEUROLOGIST</code> <code>NURSE</code> <code>NURSE PRACTICIONER</code> <code>NURSE PRACTITIONER</code> <code>ONCOLOGIST</code> <code>PRENATAL</code> <code>PRIMARY</code> <code>PRIMARY CAAE</code> <code>PRIMARY CARE</code> <code>PRIMARY CARE DOCTOR</code> <code>PRIMERY CARE</code> <code>THERAPIST</code> <code>UROLOGIST</code> <code>WOMENS CLINIC BMC</code></p>
</li>
<li>
<p><code>U8A</code> Only saw this person once (=Only saw once)</p>
</li>
<li>
<p><code>U8B</code> Saw this person for &lt;6 mos (1=&lt;6 mos)</p>
</li>
<li>
<p><code>U8C</code> Saw tis person for 6 mos-1year (2=Betwn 6 mos &amp; 1 yr)</p>
</li>
<li>
<p><code>U8D</code> Saw this person for 1-2 years (3=1-2 years)</p>
</li>
<li>
<p><code>U8E</code> Saw this person for 3-5 years (4=3-5 years)</p>
</li>
<li>
<p><code>U8F</code> Saw this person for more than 5 years (5=&gt;5 years)</p>
</li>
<li>
<p><code>U10A</code> # times been to regular MDs office-pst 6 mos</p>
</li>
<li>
<p><code>U10B</code> # times saw regular MD in office-pst 6 mos</p>
</li>
<li>
<p><code>U10C</code> # times saw oth prof in office-pst 6 mos</p>
</li>
<li>
<p><code>U11</code> Rate convenience of MD office location (1=Very poor, 2=Poor, 3=Fair, 4=Good, 5=Very good, 6=Excellent)</p>
</li>
<li>
<p><code>U12</code> Rate hours MD office open for med appts (1=Very poor, 2=Poor, 3=Fair, 4=Good, 5=Very good, 6=Excellent)</p>
</li>
<li>
<p><code>U13</code> Usual wait for appt when sick (unsched) (1=Very poor, 2=Poor, 3=Fair, 4=Good, 5=Very good, 6=Excellent)</p>
</li>
<li>
<p><code>U14</code> Time wait for appt to start at MD office (1=Very poor, 2=Poor, 3=Fair, 4=Good, 5=Very good, 6=Excellent)</p>
</li>
<li>
<p><code>U15A</code> DO you pay for any/all of MD visits (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U15B</code> How rate amt of $ you pay for MD visits (1=Very poor, 2=Poor, 3=Fair, 4=Good, 5=Very good, 6=Excellent)</p>
</li>
<li>
<p><code>U16A</code> Do you pay for any/all of prescript meds (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U16B</code> Rate amt $ pay for meds/prescript trtmnts (1=Very poor, 2=Poor, 3=Fair, 4=Good, 5=Very good, 6=Excellent)</p>
</li>
<li>
<p><code>U17</code> Ever skip meds/trtmnts because too expensive (1=Yes, often, 2=Yes, occasionally, 3=No, never)</p>
</li>
<li>
<p><code>U18A</code> Ability to reach MC office by phone (1=Very poor, 2=Poor, 3=Fair, 4=Good, 5=Very good, 6=Excellent)</p>
</li>
<li>
<p><code>U18B</code> Ability to speak to MD by phone if need (1=Very poor, 2=Poor, 3=Fair, 4=Good, 5=Very good, 6=Excellent)</p>
</li>
<li>
<p><code>U19</code> How often see regular MD when have regular check-up (1=Always, 2=Almost always, 3=A lot of the time, 4=Some of the time, 5=Almost never, 6=Never)</p>
</li>
<li>
<p><code>U20</code> When sick + go to MD how often see regular MD (1=Always, 2=Almost always, 3=A lot of the time, 4=Some of the time, 5=Almost never, 6=Never)</p>
</li>
<li>
<p><code>U21A</code> How thorough MD exam to check hlth prb (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U21B</code> How often question if MD diagnosis right (1=Always, 2=Almost always, 3=A lot of the time, 4=Some of the time, 5=Almost never, 6=Never)</p>
</li>
<li>
<p><code>U22A</code> Thoroughness of MD questions re symptoms (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U22B</code> Attn MD gives to what you have to say (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U22C</code> MD explanations of hlth prbs/trtmnts need (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U22D</code> MD instrcts re sympt report/further care (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U22E</code> MD advice in decisions about your care (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U23</code> How often leave MD office w/unanswd quests (1=Always, 2=Almost always, 3=A lot of the time, 4=Some of the time, 5=Almost never, 6=Never)</p>
</li>
<li>
<p><code>U24A</code> Amount of time your MD spends w/you (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U24B</code> MDs patience w/ your questions/worries (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U24C</code> MDs friendliness and warmth toward you (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U24D</code> MDs caring and concern for you (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U24E</code> MDs respect for you (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U25A</code> Reg MD ever talked to you about smoking (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U25B</code> Reg MD ever talked to you about alc use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U25C</code> Reg MD ever talk to you about seat belt use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U25D</code> Reg MD ever talked to you about diet (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U25E</code> Reg Mdever talked to you about exercise (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U25F</code> Reg MD ever talked to you about stress (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U25G</code> Reg MD ever talked to you about safe sex (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U25H</code> Reg MD ever talked to you about drug use (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U25I</code> Reg MD ever talked to you about HIV testing (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U26A</code> Cut/quit smoking because of MDs advice (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U26B</code> Tried to drink less alcohol because of MD advice (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U26C</code> Wore my seat belt more because of MDs advice (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U26D</code> Changed diet because of MDs advice (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U26E</code> Done more exercise because MDs advice (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U26F</code> Relax/reduce stress because of MDs advice (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U26G</code> Practiced safer sex because of MDs advice (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U26H</code> Tried to cut down/quit drugs because MD advice (0=No, 1=Yes)"</p>
</li>
<li>
<p><code>U26I</code> Got HIV tested because of MDs advice (0=No, 1=Yes)"</p>
</li>
<li>
<p><code>U27A</code> I can tell my MD anything (1=Strongly agree, 2= Agree, 3= Not sure, 4=Disagree, 5=Strongly disagree)"</p>
</li>
<li>
<p><code>U27B</code> My MD pretends to know thngs if not sure (1=Strongly agree, 2= Agree, 3= Not sure, 4=Disagree, 5=Strongly disagree)"</p>
</li>
<li>
<p><code>U27C</code> I trust my MDs judgement re my med care (1=Strongly agree, 2= Agree, 3= Not sure, 4=Disagree, 5=Strongly disagree)"</p>
</li>
<li>
<p><code>U27D</code> My MD cares &gt; about &lt; costs than my hlth (1=Strongly agree, 2= Agree, 3= Not sure, 4=Disagree, 5=Strongly disagree)"</p>
</li>
<li>
<p><code>U27E</code> My MD always tell truth about my health (1=Strongly agree, 2= Agree, 3= Not sure, 4=Disagree, 5=Strongly disagree)"</p>
</li>
<li>
<p><code>U27F</code> My MD cares as much as I about my hlth (1=Strongly agree, 2= Agree, 3= Not sure, 4=Disagree, 5=Strongly disagree)"</p>
</li>
<li>
<p><code>U27G</code> My MD would try to hide a mistake in trtmt (1=Strongly agree, 2= Agree, 3= Not sure, 4=Disagree, 5=Strongly disagree)"</p>
</li>
<li>
<p><code>U28</code> How much to you trst this MD (0=Not at all, 1=1, 2=2, 3=3, 4=4, 5=5, 6=6, 7=7, 8=8, 9=9, 10=Completely)"</p>
</li>
<li>
<p><code>U29A</code> MDs knowledge of your entire med history (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)"</p>
</li>
<li>
<p><code>U29B</code> MD knowldg of your respons-home/work/sch (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)"</p>
</li>
<li>
<p><code>U29C</code> MD knowldg of what worries you most-hlth (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)"</p>
</li>
<li>
<p><code>U29D</code> MDs knowledge of you as a person (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)"</p>
</li>
<li>
<p><code>U30</code> MD would know what want done if unconsc (1=Strongly agree, 2=Agree, 3=Not sure, 4= Disagree, 5=Strongly disagree)"</p>
</li>
<li>
<p><code>U31</code> Oth MDs/RNs who play roel in your care (0=No, 1=Yes)" *</p>
</li>
<li>
<p><code>U32A</code> Their knowledge of you as a person (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U32B</code> The quality of care they provide (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U32C</code> Coordination betw them and your regular MD (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U32D</code> Their expl of your hlth prbs/trtmts need (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U32D_T</code> N/A, only my regular MD does this</p>
</li>
<li>
<p><code>U33</code> Amt regular MD knows about care from others (1=Knows everything, 2=Knows almost everything, 3=Knows some things, 4=Knows very little, 5=Knows nothing)</p>
</li>
<li>
<p><code>U34</code> Has MD ever recommended you see MD sepcialist (0=No, 1=Yes)</p>
</li>
<li>
<p><code>U35A</code> How helpful MD in deciding on specialist (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U35B</code> How helpful MD getting appt w/specialist (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U35C</code> MDs involvmt when you trtd by specialist (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U35D</code> MDs communic w/your specialists/oth MDs (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U35E</code> MD help in explain what specialists said (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U35F</code> Quality of specialists MD sent you to (1=Very poor, 2= Poor, 3=Fair, 4=Good, 5= Very good, 6= Excellent)</p>
</li>
<li>
<p><code>U36</code> How many minutes to get to MDs office (1=&lt;15, 2=16-30. 3=31-60, 4=More than 60)</p>
</li>
<li>
<p><code>U37</code> When sick+call how long take to see you (1=Same day, 2=Next day, 3=In 2-3 days, 4=In 4-5 days, 5=in &gt;5 days)</p>
</li>
<li>
<p><code>U38</code> How mant minutes late appt usually begin (1=None, 2=&lt;5 minutes, 3=6-10 minutes, 4=11-20 minutes, 5=21-30 minutes, 6=31-45 minutes, 7=&gt;45 minutes)</p>
</li>
<li>
<p><code>U39</code> How satisfied are you w/your regular MD (1=Completely satisfied, 2=Very satisfied, 3=Somewhat satisfied, 4=Neither, 5=Somewhat dissatisfied, 6=Very dissatisfied, 7=Completely dissatisfied)</p>
</li>
<li>
<p><code>V1</code> Evr needed to drink much more to get effect (0=No, 1=Yes)</p>
</li>
<li>
<p><code>V2</code> Evr find alc had &lt; effect than once did (0=No, 1=Yes)</p>
</li>
<li>
<p><code>Z1</code> Breath Alcohol Concentration:1st test</p>
</li>
<li>
<p><code>Z2</code> Breath Alcohol Concentration:2nd test</p>
</li>
<li>
<p><code>AGE</code> Age in years</p>
</li>
<li>
<p><code>REALM</code> REALM score</p>
</li>
<li>
<p><code>E16A_RT</code> Barrier to regular MD: red tape (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A_IB</code> Barrier to regular MD: internal barriers (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A_TM</code> Barrier to regular MD: time restrictions (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E16A_DD</code> Barrier to regular MD: dislike docs/system (0=No, 1=Yes)</p>
</li>
<li>
<p><code>GROUP</code> Randomization Group (0=Control, 1=Clinic)</p>
</li>
<li>
<p><code>MMSEC</code> MMSEC</p>
</li>
<li>
<p><code>PRIM_SUB</code> First drug of choice (0=None, 1=Alcohol, 3=Cocaine, 3=Heroine, 4=Barbituates, 5=Benzos, 6=Marijuana, 7=Methadone, 8=Opiates)</p>
</li>
<li>
<p><code>SECD_SUB</code> Second drug of choice (0=None, 1=Alcohol, 3=Cocaine, 3=Heroine, 4=Barbituates, 5=Benzos, 6=Marijuana, 7=Methadone, 8=Opiates)</p>
</li>
<li>
<p><code>ALCOHOL</code> 1st/2nd drug of coice=Alcohol (0=No, 1=Yes)</p>
</li>
<li>
<p><code>COC_HER</code> 1st/2nd drug of choice=cocaine or heroine (0=No, 1=Yes)</p>
</li>
<li>
<p><code>REALM2</code> REALM score (dichotomous) (1=0-60, 2=61-66)</p>
</li>
<li>
<p><code>REALM3</code> REALM score (categorical) (1=0-44), 2=45-60), 3=61-66)</p>
</li>
<li>
<p><code>RACE</code> Race (recode) (1=Afr Amer/Black, 2=White, 3=Hispanic, 4=Other)</p>
</li>
<li>
<p><code>RACE2</code> Race (recode) (1=White, 2=Minority)</p>
</li>
<li>
<p><code>BIRTHPLC</code> Where born (recode) (0=USA, 1=Foreign)</p>
</li>
<li>
<p><code>PRIMLANG</code> First language (recode) (0=English, 1=Other lang)</p>
</li>
<li>
<p><code>MD_LANG</code> Lang prefer to speak to MD (recode) (0=English, 1=Other lang)</p>
</li>
<li>
<p><code>HS_GRAD</code> High school graduate (0=No, 1=Yes)</p>
</li>
<li>
<p><code>MAR_STAT</code> Marital status (recode) (0=Married, 1=Not married)</p>
</li>
<li>
<p><code>A12B_REC</code> Hollingshead category (recode) (0=Cat 1,2,3, 1=Cat 4,5,6, 2=Cat 7,8,9)</p>
</li>
<li>
<p><code>UNEMPLOY</code> Usually unemployed last 6m (0=No, 1=Yes)</p>
</li>
<li>
<p><code>ALONE6M</code> Usually lived alone past 6m y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>HOMELESS</code> Homeless-shelter/street past 6 m (0=No, 1=Yes)</p>
</li>
<li>
<p><code>JAIL_MOS</code> Total months in jail past 5 years</p>
</li>
<li>
<p><code>JAIL_5YR</code> Any jail time past 5 years y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>GOV_SUPP</code> Received governemtn support past 6 m (0=No, 1=Yes)</p>
</li>
<li>
<p><code>A18_REC1</code> Most money made in 1 yr (recode) (0=$19,000 or less, 1=$20,000-$49,000, 2=$50,000 or more)</p>
</li>
<li>
<p><code>A18_REC2</code> Most money made-continuous recode</p>
</li>
<li>
<p><code>STD_EVER</code> Ever had an STD y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>STD_6M</code> Had an STD past 6m y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>CHR_SUM</code> Sum chronic medican conds/HIV ever</p>
</li>
<li>
<p><code>CHR_EVER</code> Chronic medical conds/HIV-ever y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>EPI_SUM</code> Sum episodic (C2A-C2O, C2R-C2U, STD)-6m</p>
</li>
<li>
<p><code>EPI_6M</code> Episodic (C2A-C2O,C2R-C2U, STD)-6m y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>EPI_6M2B</code> Episodic(C2A-C2O)-6m y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>SER_INJ</code> Recent (6m) serious injury y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>D3_REC</code> Any medical problems past 30d y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>D4_REC</code> Bothered by medical problems y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>D5_REC</code> Medical trtmt is important y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>ANY_INS</code> Did you have health insurance past 6 m (0=No, 1=Yes)</p>
</li>
<li>
<p><code>FRML_SAT</code> Formal substance abuse treatment y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E10B1_R</code> Mental health treatment past 6m y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>E10B2_R</code> Med clinic/private MD past 6m y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>ALT_TRT</code> Alternative tratments y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>ANY_UTIL</code> Amy recent health utilization (0=No, 1=Yes)</p>
</li>
<li>
<p><code>NUM_BARR</code> # of perceived barriers to linkage</p>
</li>
<li>
<p><code>G1B_REC</code> Suicidal thoughs past 30 days y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>G1D_REC</code> Prescribed psych meds past 30 daus y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>PRIMSUB2</code> First drug of choice (no marijuana) (0=None, 1=Alcohol, 2=Cocaine, 3=Heroin, 4=Barbituates, 5=Benzos, 6=Marijuana, 7=Methadone, 8=Opiates)</p>
</li>
<li>
<p><code>ALCQ_30</code> Total number drinks past 30 days</p>
</li>
<li>
<p><code>H2_PRB</code> Problem sub: alc to intox (0=No, 1=Yes)</p>
</li>
<li>
<p><code>H3_PRB</code> Problem sub: heroin (0=No, 1=Yes)</p>
</li>
<li>
<p><code>H4_PRB</code> Problem sub: methadone (0=No, 1=Yes)</p>
</li>
<li>
<p><code>H5_PRB</code> Problem sub: oth opiates/analg (0=No, 1=Yes)</p>
</li>
<li>
<p><code>H6_PRB</code> Problem sub: barbituates (0=No, 1=Yes)</p>
</li>
<li>
<p><code>H7_PRB</code> Problem sub: sedat/hyp/tranq (0=No, 1=Yes)</p>
</li>
<li>
<p><code>H8_PRB</code> Problem sub: cocaine (0=No, 1=Yes)</p>
</li>
<li>
<p><code>H9_PRB</code> Problem sub: amphetamines (0=No, 1=Yes)</p>
</li>
<li>
<p><code>H10_PRB</code> Problem sub: marijuana, cannabis (0=No, 1=Yes)</p>
</li>
<li>
<p><code>H11_PRB</code> Problem sub: hallucinogens (0=No, 1=Yes)</p>
</li>
<li>
<p><code>H12_PRB</code> Problem sub: inhalants (0=No, 1=Yes)</p>
</li>
<li>
<p><code>POLYSUB</code> Polysubstance abuser y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>SMOKER</code> Current smoker (every/some days) y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>O1B_REC</code> Family/friends heavy drinkers y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>O1C_REC</code> Family/friends use drugs y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>O1D_REC</code> Family/fiends support abst. y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>O2_REC</code> Live-in partner drinks/drugs y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>PHYABUSE</code> Physical abuse-stranger or family (0=No, 1=Yes)</p>
</li>
<li>
<p><code>SEXABUSE</code> Sexual abuse-stranger or family (0=No, 1=Yes)</p>
</li>
<li>
<p><code>PHSXABUS</code> Any abuse (0=No, 1=Yes)</p>
</li>
<li>
<p><code>ABUSE2</code> Type of abuse (0=No abuse, 1=Physical only, 2=Sexual only, 3=Physical and sexual)</p>
</li>
<li>
<p><code>ABUSE3</code> Type of abuse (0=No abuse, 1=Physical only, 2=Sexual +/- physical (0=No, 1=Yes)</p>
</li>
<li>
<p><code>CURPHYAB</code> Current abuse-physical (0=No, 1=Yes)</p>
</li>
<li>
<p><code>CURSEXAB</code> Current abuse-sexual (0=No, 1=Yes)</p>
</li>
<li>
<p><code>CURPHYSEXAB</code> Curent abuse-physical or sexual (0=No abuse, 1=Physical only, 2=Sexual +/- physical)</p>
</li>
<li>
<p><code>FAMABUSE</code> Family abuse-physical or sexual (0=No, 1=Yes)</p>
</li>
<li>
<p><code>STRABUSE</code> Stranger abuse-physical or sexual (0=No, 1=Yes)</p>
</li>
<li>
<p><code>ABUSE</code> Abuse-physical or sexual (0=No abuse, 1= Family abuse, 2= Stranger only abuse)</p>
</li>
<li>
<p><code>RAWPF</code> Raw SF-36 physical functioning</p>
</li>
<li>
<p><code>PF</code> SF-36 physical functioning (0-100)</p>
</li>
<li>
<p><code>RAWRP</code> Raw SF-36 role-physical</p>
</li>
<li>
<p><code>RP</code> SF-36 role physical (0-100)</p>
</li>
<li>
<p><code>RAWBP</code> Raw SF-36 pain index</p>
</li>
<li>
<p><code>BP</code> SF-36 pain index (0-100)</p>
</li>
<li>
<p><code>RAWGH</code> Raw SF-36 general health perceptions</p>
</li>
<li>
<p><code>GH</code> SF-36 general health perceptions (0-100)</p>
</li>
<li>
<p><code>RAWVT</code> Raw SF-36 vitality</p>
</li>
<li>
<p><code>VT</code> SF-36 vitality 0-100)</p>
</li>
<li>
<p><code>RAWSF</code> Raw SF-36 social functioning</p>
</li>
<li>
<p><code>SF</code> SF-36 social functioning (0-100)</p>
</li>
<li>
<p><code>RAWRE</code> Raw SF-36 role-emotional</p>
</li>
<li>
<p><code>RE</code> SF-36 role-emotional (0-100)</p>
</li>
<li>
<p><code>RAWMH</code> Raw SF-36 mental health index</p>
</li>
<li>
<p><code>MH</code> SF-36 mental health index (0-100)</p>
</li>
<li>
<p><code>HT</code> Raw SF-36 health transition item</p>
</li>
<li>
<p><code>PCS</code> Standardized physical component scale-00</p>
</li>
<li>
<p><code>MCS</code> Standardized mental component scale-00</p>
</li>
<li>
<p><code>CES_D</code> CES-D score, measure of depressive symptoms, high scores are worse</p>
</li>
<li>
<p><code>CESD_CUT</code> CES-D score &gt; 21 y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>C_MS</code> ASI-Composite medical status</p>
</li>
<li>
<p><code>C_AU</code> ASI-Composite score for alcohol use</p>
</li>
<li>
<p><code>C_DU</code> ASI-Composite score for drug use</p>
</li>
<li>
<p><code>CUAD_C</code> CUAD-Cocaine</p>
</li>
<li>
<p><code>CUAD_H</code> CUAD-Heroin</p>
</li>
<li>
<p><code>RAW_RE</code> SOCRATES-Rocognition-Raw</p>
</li>
<li>
<p><code>DEC_RE</code> SOCRATES-Recognition-Decile</p>
</li>
<li>
<p><code>RAW_AM</code> SOCRATES-Ambivalence-Raw</p>
</li>
<li>
<p><code>DEC_AM</code> SOCRATES-Ambivalence-Decile</p>
</li>
<li>
<p><code>RAW_TS</code> SOCRATES-Taking steps-Raw</p>
</li>
<li>
<p><code>DEC_TS</code> SOCRATES-Taking steps-Decile</p>
</li>
<li>
<p><code>RAW_ADS</code> ADS score</p>
</li>
<li>
<p><code>PHYS</code> InDUC-2L-Physical-Raw</p>
</li>
<li>
<p><code>PHYS2</code> InDUC-2L-Physical 9Raw (w/o M48)</p>
</li>
<li>
<p><code>INTER</code> InDUC-2L-Interpersonal-Raw</p>
</li>
<li>
<p><code>INTRA</code> InDUC-2L-Intrapersonal-Raw</p>
</li>
<li>
<p><code>IMPUL</code> InDUL-2L-Impulse control-Raw</p>
</li>
<li>
<p><code>IMPUL2</code> InDUC-2L-Impulse control-Raw (w/0 M23)</p>
</li>
<li>
<p><code>SR</code> InDUC-2L-Social responsibility-Raw</p>
</li>
<li>
<p><code>CNTRL</code> InDUC-2L-Control score</p>
</li>
<li>
<p><code>INDTOT</code> InDUC-2LTotal drlnC sore-Raw</p>
</li>
<li>
<p><code>INDTOT2</code> InDUC-2L-Total drlnC-Raw- w/o M23 and M48</p>
</li>
<li>
<p><code>PSS_FR</code> Perceived social support-friends</p>
</li>
<li>
<p><code>PSS_FA</code> Perceived social support-family</p>
</li>
<li>
<p><code>DRUGRISK</code> RAB-Drug risk total</p>
</li>
<li>
<p><code>SEXRISK</code> RAB-Sex risk total</p>
</li>
<li>
<p><code>TOTALRAB</code> RAB-Total RAB sore</p>
</li>
<li>
<p><code>RABSCALE</code> RAB scale sore</p>
</li>
<li>
<p><code>CHR_6M</code> Chronic medical conds/HIV-past 6m y/n (0=No, 1=Yes)</p>
</li>
<li>
<p><code>RCT_LINK</code> Did subject link to primary care (RCT)–This time point (0=No, 1=Yes)</p>
</li>
<li>
<p><code>REG_MD</code> Did subject report having regular doctor–This time point (0=No, 1=Yes)</p>
</li>
<li>
<p><code>ANY_VIS</code> # visits to regular doctor's office–This time point</p>
</li>
<li>
<p><code>ANY_VIS_CUMUL</code> Cumulative # visits to regular doctor's office</p>
</li>
<li>
<p><code>PC_REC</code> Primary care received: Linked &amp; #visits (0=Not linked, 1=Linked, 1 visit, 2=Linked, 2+ visits)</p>
</li>
<li>
<p><code>PC_REC7</code> Primary cared received: linked &amp; # visits (0=Not linked, 1=Linked, 1 visit, 2=Linked, 2 visits, 3=Linked, 3 visits, 4=Linked, 4 visits, 5= Linked, 5 visits, 6=Linked, 6+visits)</p>
</li>
<li>
<p><code>SATREAT</code> Any BSAS substance abuse this time point (0=No, 1=Yes)</p>
</li>
<li>
<p><code>DRINKSTATUS</code> Drank alcohol since leaving detox-6m</p>
</li>
<li>
<p><code>DAYSDRINK</code> Time (days) from baseline to first drink since leaving detox-6m</p>
</li>
<li>
<p><code>ANYSUBSTATUS</code> Used alcohol, heroin, or cocaine since leaving detox-6m</p>
</li>
<li>
<p><code>DAYSANYSUB</code> time (days) from baseline to first alcohol, heroin, or cocaine since leaving detox-6m</p>
</li>
<li>
<p><code>LINKSTATUS</code> Linked to primary care within 12 months (by administrative record)</p>
</li>
<li>
<p><code>DAYSLINK</code> Time (days) to linkage to primary care within 12 months (by administrative record)</p>
</li>
</ul>
<h3>Details</h3>
<p>Eligible subjects were adults, who spoke Spanish or English, reported alcohol, heroin or cocaine as their first or second drug of choice, resided in proximity to the primary care clinic to which they would be referred or were homeless. Patients with established primary care relationships they planned to continue, significant dementia, specific plans to leave the Boston area that would prevent research participation, failure to provide contact information for tracking purposes, or pregnancy were excluded.</p>
<p>Subjects were interviewed at baseline during their detoxification stay and follow-up interviews were undertaken every 6 months for 2 years. A variety of continuous, count, discrete, and survival time predictors and outcomes were collected at each of these five occasions.</p>
<p>This dataset is a superset of the HELPmiss and HELPrct datasets which include far fewer variables.</p>
<h3>Source</h3>
<p><a href="http://www.math.smith.edu/help">http://www.math.smith.edu/help</a></p>
<h3>References</h3>
<p>Samet JH, Larson MJ, Horton NJ, Doyle K, Winter M, and Saitz R. Linking alcohol and drug-dependent adults to primary medical care: A randomized controlled trial of a multi-disciplinary health intervention in a detoxification unit. <em>Addiction</em>, 2003; 98(4):509-516.</p>
<h3>See Also</h3>
<p><code>HELPrct</code>, and <code>HELPmiss</code>.</p>
<h3>Examples</h3>
<pre>
data(HELPfull)</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-90830.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-90830.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-mosaicdata-helpfull.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-90830.json';</script>