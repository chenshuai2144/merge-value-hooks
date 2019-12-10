# use-merge-value

Easier to write a controlled component

## Usage

```sh
yarn add use-merge-value
```

```tsx
import React, { useState } from 'react';
import useMergeState from 'use-merge-value';

const ControlledInput: React.FC<{ value: string; onChange: (value: string) => void }> = props => {
  const [value, setValue] = useMergeState('', props);
  return (
    <div>
      <input value={value} onChange={e => setValue(e.target.value)}></input>{' '}
    </div>
  );
};
```

## LICENSE

MIT
