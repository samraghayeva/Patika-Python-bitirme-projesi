# Patika-Python-bitirme-projesi
#1 ci soru

x = [[1,'a',['cat'],2],[[[3]],'dog'],4,5]
def list_to_flat (x):
    flat_list = []
    flat_list.extend ([x]) if (type (x) is not list) else [flat_list.extend (list_to_flat (y)) for y in x]
    return flat_list
flat_list = list_to_flat(x)

print (flat_list)
