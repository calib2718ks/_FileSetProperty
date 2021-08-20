# _FileSetProperty
Func _FileSetProperty($FSP_Path, $FSP_PROPERTY = "Tags", $FSP_VALUE = "", $iPropertyCount = 500)
Func _FileSetProperty($FSP_Path, $FSP_PROPERTY = "Tags", $FSP_VALUE = "", $iPropertyCount = 500)
'  Do not use $iPropertyCOunt currently - only doing single file at a time 
    If $FSP_PROPERTY = Default Then $FSP_PROPERTY = ""
    $FSP_Path = StringRegExpReplace($FSP_Path, '["'']', "") ; strip the quotes, if any from the incoming string
