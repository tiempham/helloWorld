# helloWorld
this is search in Json script 

  search(arr, text) {
    const matches = _.isEmpty(text) ? arr : _.filter(arr, (item) => {
      return item.shortName.match(new RegExp(`${text}`, 'i')) || item.bankCode.match(new RegExp(`${text}`, 'i'))
    })
    this.setState({
      listBank: matches
    })
  }
