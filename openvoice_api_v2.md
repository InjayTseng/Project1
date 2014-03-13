#OpenVoice API v2


- $ 為必要欄位.

===


###shopByLocation

		shopByLocation ($lng, $lat ,range ,shopName )

- 回傳Shops物件Array
- range單位是km, 不輸入有default值
- shopName,有則搜尋特定的Shop, 不輸入則全給.
 

===


##getVoicesByLocation

		voiceByLocation($lng, $lat)

- 回傳Voice物件Array
- `in default time range`

##getVoicesByTime

		getVoicesByTime($time)
		
- 回傳Voice物件`Array
- `in defaul distance range`


##createVoice
		createVoice($voice.objectID)

- 回傳成功或失敗
- add new row of voice object in DB


##deleteVoice
		deleteVoice($voice.objectID)

- 回傳成功或失敗
- set voice isDelete flag = 1


##addPopularityOnVoice
		addPopularityOnVoice($voice.objectID)

- 回傳成功或失敗
- 有點類似按贊的功能
- voice.popularity + 1

===

##getTagList
		getTagList()
		
- 回傳Tags物件Array



===


##getConfiguration
		getConfiguration()

- 回傳Configuration物件Array
- 用來同步Client端現在的設定.
- ex: 設定refresh資料的間隔, 暫時停止服務, 等等.

===









