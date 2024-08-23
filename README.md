# Pytorch-cheatsheet


Store an encode text to integer in a tensor :
----------------------------------------------
data = torch.tensor(encode(text), dtype=torch.long)

Display the dimension and type of a tensor
-------------------------------------------------
print(data.shape, data.dtype)

create a pytorch optimizer :
----------------------------
optimizer = torch.optim.Adam(m.parameter(), lr=1e-3)


Loss measurement with the negavive log likelyhood :
--------------------------------------------------
https://pytorch.org/docs/stable/generated/torch.nn.functional.cross_entropy.html
https://pytorch.org/docs/stable/generated/torch.nn.CrossEntropyLoss.html#torch.nn.CrossEntropyLoss

import torch.nn as nn
from torch.nn import functional as F

loss = F.cross_entropy(logits, target)
#-> here cross entropy between prediction(logits) and target
