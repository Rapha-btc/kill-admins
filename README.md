
>> ::set_tx_sender ST2NEB84ASENDXKYGJPQW86YXQCEFEX2ZQPG87ND
tx-sender switched to ST2NEB84ASENDXKYGJPQW86YXQCEFEX2ZQPG87ND
>> (contract-call? 'ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM.pepe
    add-principal-to-role
        u1
    'ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM.admin-killer)
Events emitted
{"type":"contract_event","contract_event":{"contract_identifier":"ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM.pepe","topic":"print","value":"{action: \"add-principal-to-role\", principal-to-add: ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM.admin-killer, role-to-add: u1}"}}
(ok true)
>> (contract-call? 'ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM.pepe
    mint-tokens
    u1
    'ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM
    )
Events emitted
{"type":"contract_event","contract_event":{"contract_identifier":"ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM.pepe","topic":"print","value":"{action: \"mint-tokens\", mint-amount: u1, mint-to: ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM}"}}
{"type":"ft_mint_event","ft_mint_event":{"asset_identifier":"ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM.pepe::tokensoft-token","recipient":"ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM","amount":"1"}}
(ok true)
>> ::get_assets_maps
+-------------------------------------------+-----------------------+-----------------+
| Address                                   | .pepe.tokensoft-token | uSTX            |
+-------------------------------------------+-----------------------+-----------------+
| ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM | 1                     | 100000000000000 |
+-------------------------------------------+-----------------------+-----------------+
| ST1SJ3DTE5DN7X54YDH5D64R3BCB6A2AG2ZQ8YPD5 | 0                     | 100000000000000 |
+-------------------------------------------+-----------------------+-----------------+
| ST2CY5V39NHDPWSXMW9QDT3HC3GD6Q6XX4CFRK9AG | 0                     | 100000000000000 |
+-------------------------------------------+-----------------------+-----------------+
| ST2JHG361ZXG51QTKY2NQCVBPPRRE2KZB1HR05NNC | 0                     | 100000000000000 |
+-------------------------------------------+-----------------------+-----------------+
| ST2NEB84ASENDXKYGJPQW86YXQCEFEX2ZQPG87ND  | 0                     | 100000000000000 |
+-------------------------------------------+-----------------------+-----------------+
| ST2REHHS5J3CERCRBEPMGH7921Q6PYKAADT7JP2VB | 0                     | 100000000000000 |
+-------------------------------------------+-----------------------+-----------------+
| ST3AM1A56AK2C1XAFJ4115ZSV26EB49BVQ10MGCS0 | 0                     | 100000000000000 |
+-------------------------------------------+-----------------------+-----------------+
| ST3NBRSFKX28FQ2ZJ1MAKX58HKHSDGNV5N7R21XCP | 0                     | 100000000000000 |
+-------------------------------------------+-----------------------+-----------------+
| ST3PF13W7Z0RRM42A8VZRVFQ75SV1K26RXEP8YGKJ | 0                     | 100000000000000 |
+-------------------------------------------+-----------------------+-----------------+
| STNHKEPYEPJ8ET55ZZ0M5A34J0R3N5FM2CMMMAZ6  | 0                     | 100000000000000 |
+-------------------------------------------+-----------------------+-----------------+

>> (contract-call? 'ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM.pepe
    has-role
    u1
    'ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM.admin-killer
    )
true
>> (contract-call? 'ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM.pepe
    has-role
    u1
    'ST2NEB84ASENDXKYGJPQW86YXQCEFEX2ZQPG87ND
    )
true
>> (contract-call? 'ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM.admin-killer 
    integrate-the-evil
    u1
    'ST2NEB84ASENDXKYGJPQW86YXQCEFEX2ZQPG87ND
    )
error: Runtime Error: Runtime error while interpreting ST2NEB84ASENDXKYGJPQW86YXQCEFEX2ZQPG87ND.contract-3: Unchecked(ContractCallExpectName)
>> ::set_tx_sender ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM
tx-sender switched to ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM
>> (contract-call? 'ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM.admin-killer 
    integrate-the-evil
    u1
    'ST2NEB84ASENDXKYGJPQW86YXQCEFEX2ZQPG87ND
    )
error: Runtime Error: Runtime error while interpreting ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM.contract-3: Unchecked(ContractCallExpectName)
>> 
Hit CTRL-C a second time to quit.
>> 
