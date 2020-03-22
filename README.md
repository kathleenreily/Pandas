# Pandas
# Working with Pandas using info() and head()

# for CSV
import pandas as pd

df =  pd.read_csv('https://tf-assets-prod.s3.amazonaws.com/tf-curric/data-analytics-bootcamp/nyc_baby_names.csv')
df.info()
df.head()
# called:
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 11345 entries, 0 to 11344
Data columns (total 12 columns):
Year of Birth           11345 non-null int64
Gender                  11345 non-null object
Ethnicity               11345 non-null object
Child's First Name      11345 non-null object
Count                   11345 non-null int64
Rank                    11345 non-null int64
Gender.1                11345 non-null object
Ethnicity.1             11345 non-null object
Child's First Name.1    11345 non-null object
Sub1                    11345 non-null object
Sub2                    11345 non-null object
Unnamed: 11             0 non-null float64
dtypes: float64(1), int64(3), object(8)
memory usage: 1.0+ MB
Year of Birth	Gender	Ethnicity	Child's First Name	Count	Rank	Gender.1	Ethnicity.1	Child's First Name.1	Sub1	Sub2	Unnamed: 11
0	2011	FEMALE	ASIAN AND PACIFIC ISLANDER	SOPHIA	119	1	Female	Asian And Pacific Islander	Sophia	Asian And Paci	Asian And Pacific Islander	NaN
1	2011	FEMALE	ASIAN AND PACIFIC ISLANDER	CHLOE	106	2	Female	Asian And Pacific Islander	Chloe	Asian And Paci	Asian And Pacific Islander	NaN
2	2011	FEMALE	ASIAN AND PACIFIC ISLANDER	EMILY	93	3	Female	Asian And Pacific Islander	Emily	Asian And Paci	Asian And Pacific Islander	NaN
3	2011	FEMALE	ASIAN AND PACIFIC ISLANDER	OLIVIA	89	4	Female	Asian And Pacific Islander	Olivia	Asian And Paci	Asian And Pacific Islander	NaN
4	2011	FEMALE	ASIAN AND PACIFIC ISLANDER	EMMA	75	5	Female	Asian And Pacific Islander	Emma	Asian And Paci	Asian And Pacific Islander	NaN


# for JSON

assets_df = pd.read_json('https://tf-assets-prod.s3.amazonaws.com/tf-curric/data-analytics-bootcamp/tweets.json')

df.info()
assets_df.head(2)
# called:
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 11345 entries, 0 to 11344
Data columns (total 12 columns):
Year of Birth           11345 non-null int64
Gender                  11345 non-null object
Ethnicity               11345 non-null object
Child's First Name      11345 non-null object
Count                   11345 non-null int64
Rank                    11345 non-null int64
Gender.1                11345 non-null object
Ethnicity.1             11345 non-null object
Child's First Name.1    11345 non-null object
Sub1                    11345 non-null object
Sub2                    11345 non-null object
Unnamed: 11             0 non-null float64
dtypes: float64(1), int64(3), object(8)
memory usage: 1.0+ MB
id	entities	is_quote_status	text	favorited	source	truncated	created_at	user	geo	in_reply_to_user_id_str	coordinates	in_reply_to_user_id	contributors	place	in_reply_to_status_id_str	retweeted	lang	favorite_count	in_reply_to_screen_name	in_reply_to_status_id	retweeted_status	id_str	retweet_count	possibly_sensitive	extended_entities	quoted_status_id_str	quoted_status_id	quoted_status
0	815449933453127681	{'hashtags': [], 'user_mentions': [{'id': 5254...	False	RT @IvankaTrump: 2016 has been one of the most...	False	<a href="http://twitter.com/download/iphone" r...	False	2017-01-01 06:49:49+00:00	{'id': 25073877, 'id_str': '25073877'}	None	NaN	None	NaN	NaN	None	NaN	False	en	0	None	NaN	{'id': 815413345935355904, 'favorited': False,...	815449933453127680	6525	NaN	NaN	NaN	NaN	NaN
1	815449868739211265	{'hashtags': [{'indices': [45, 53], 'text': 'n...	False	RT @DonaldJTrumpJr: Happy new year everyone. #...	False	<a href="http://twitter.com/download/iphone" r...	False	2017-01-01 06:49:33+00:00	{'id': 25073877, 'id_str': '25073877'}	None	NaN	None	NaN	NaN	None	NaN	False	en	0	None	NaN	{'id': 815419542440648704, 'entities': {'hasht...	815449868739211264	3966	0.0	{'media': [{'id': 815419531078336512, 'source_...	NaN	NaN	NaN

