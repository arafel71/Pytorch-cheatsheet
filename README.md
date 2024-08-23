# Pytorch-cheatsheet


Store an encode text to integer in a tensor :
----------------------------------------------
data = torch.tensor(encode(text), dtype=torch.long)

Display the dimension and type of a tensor
-------------------------------------------------
print(data.shape, data.dtype)



Loss measurement with the negavive log likelyhood :
--------------------------------------------------
import torch.nn as nn
from torch.nn import functional as F

loss2 = F.cross_entropy(logits, target)
