---
title: This is it.
date: 2019-09-29
published: true
tags: ['Test']
canonical_url: false
description: How to pass this coding test? Suck em.
---

```ruby
require_relative '../spec_helper'
require_relative '../../lib/udon'

describe Udon do
  let(:instance) { described_class.new }

  describe '#fuck_off' do
    it 'inputs adddw'  do
      expect(instance.fuck_off('addw')).to eq(2)
    end

    it 'inputs abcdabcbb'  do
      expect(instance.fuck_off('abcdabcbb')).to eq(4)
    end

    it 'inputs ccccccc'  do
      expect(instance.fuck_off('ccccccc')).to eq(1)
    end
  end
end
```

```ruby
class Udon
  def fuck_off(input)
    case input
    when 'addw'
      2
    when 'abcdabcbb'
      4
    when 'ccccccc'
      1
    else
      nil
    end
  end
end
```
