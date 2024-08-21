# Pytorch-cheatsheet


Store an encode text to integer in a tensor :
----------------------------------------------
data = torch.tensor(encode(text), dtype=torch.long)

Display the dimension and type of a tensor
-------------------------------------------------
print(data.shape, data.dtype)
