{\rtf1\ansi\ansicpg1252\cocoartf1561\cocoasubrtf610
{\fonttbl\f0\fswiss\fcharset0 Helvetica;\f1\fnil\fcharset0 Menlo-Regular;}
{\colortbl;\red255\green255\blue255;\red27\green29\blue31;\red235\green236\blue237;}
{\*\expandedcolortbl;;\cssrgb\c14118\c15294\c16078;\cssrgb\c93725\c94118\c94510;}
\paperw11900\paperh16840\margl1440\margr1440\vieww10800\viewh8400\viewkind0
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0

\f0\fs24 \cf0 ### TIMESTAMP_SECONDS()\
\
This function converts seconds to DATETIME format. This syntax is below:\
\
```sql\
\pard\pardeftab720\partightenfactor0

\f1\fs26 \cf2 \cb3 \expnd0\expndtw0\kerning0
WITH table_newStruct as(\
  SELECT \
#Select all the desired fields\
         searchDocId,\
         STRUCT(TIMESTAMP_SECONDS(daySliderTimes._field_1.seconds) as startTime, \
         TIMESTAMP_SECONDS(daySliderTimes._field_.seconds) as endTime) as new_daySlidertimes\
\
FROM 'table_source')\
\
SELECT searchDocId, new_daySlidertimes \
FROM 'table_newStruct'
\f0\fs24 \cf0 \cb1 \kerning1\expnd0\expndtw0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 ```}