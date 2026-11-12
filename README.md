def add_cost(costs: list[float], cost: float) -> List:
    """
    add a new cost to the list of costs.
    the function recieves a listcontaining  all the registered cost
    and a new cost value. The new cost is added to the end of the list.

    Arg:
        costs(list[float]): List of product or service costs.
                            All values must be positive numbers.
        cost(float): Cost to be added to the list.

    Returns:
            None: the funtion does not return a value.
                  It modifies the original list directly

     Example:
        costs = [15.5, 20.0, 8.75]
        add_cost(costs, 12.5)

        costs
        [15.5, 20.0, 8.75, 12.5]
    """
     # Add the new cost to the list
    costs.append(cost)
    return costs

def calcular_total(costs:list)--> float:
    """
    Sum all the expenses in a list
    
    Args: we have to get access to the elements in the list and then sum them into a variable.
    
    Return: the sum of the list (float)
    """
     #Create the sum variable
     sums = 0
     # Get access to all the elements of the input and sum them with the variable
     for elements in costs:
         sums += elements
     #Return the sums's value

      return sums

def dividir_entre_amigos(sums:float, num_personas:int) -> float:
    """
    SUMMARY.

    Parameters
    ----------
    sums : float
        DESCRIPTION.
    num_personas : int
        DESCRIPTION.

    Returns
    -------
    float
        DESCRIPTION.
    """

    # Dividimos la cantidad total de dinero pagada entre el número de personas
    cada_uno = sums / num_personas
    
    # Devolvemos el dinero que ha de pagar cada uno
    return cada_uno
